# Análise de Vendas Mensais, Lucro por Departamento e Modos de Envio em São Paulo

Este projeto realiza a análise das vendas mensais, lucro por departamento e modos de envios mais utilizados em São Paulo. Ele cria gráficos a partir dos dados, exporta os resultados para arquivos Excel e gera um relatório PDF.

## Sumário

- [Descrição](#descrição)
- [Pré-requisitos](#pré-requisitos)
- [Instalação](#instalação)
- [Uso](#uso)
- [Funções](#funções)
- [Contribuição](#contribuição)
- [Licença](#licença)
- [Contato](#contato)

## Descrição

Este projeto foi desenvolvido para analisar os dados de vendas mensais, lucro por departamento e modos de envio mais utilizados em São Paulo. Ele gera gráficos ilustrativos, exporta os dados processados para arquivos Excel e gera um relatório PDF detalhado. O principal objetivo é fornecer visualizações claras e compreensíveis das tendências e padrões encontrados nos dados.

## Pré-requisitos

Antes de começar, certifique-se de que você tem os seguintes requisitos atendidos:
- Python 3.6 ou superior
- Pandas
- Matplotlib
- Openpyxl
- FPDF

## Instalação

1. Clone este repositório:
    ```bash
    git clone https://github.com/seu_usuario/seu_repositorio.git
    ```

2. Navegue para o diretório do projeto:
    ```bash
    cd seu_repositorio
    ```

3. Crie e ative um ambiente virtual (opcional, mas recomendado):
    ```bash
    python -m venv env
    source env/bin/activate  # Para Windows, use `env\Scripts\activate`
    ```

4. Instale as dependências:
    ```bash
    pip install pandas matplotlib openpyxl fpdf
    ```

## Uso

1. Execute o script principal para processar os dados, gerar os gráficos e criar o relatório PDF:
    ```bash
    python script_principal.py
    ```

2. O script exportará arquivos Excel chamados `vendas_por_mes.xlsx`, `lucro_por_departamento.xlsx` e `modos_envio_sp.xlsx`, além de salvar os gráficos correspondentes como `vendas_por_mes.png`, `lucro_por_departamento.png` e `modos_envio_sp.png`. Ele também gerará um relatório PDF chamado `Relatório_2023.pdf`.

## Funções

### `grafico_vendas_por_mes`

Esta função cria um gráfico das vendas mensais.

```python
def grafico_vendas_por_mes(df, filename):
    df["vendas_numerico"] = df["vendas"].str.replace("R\$", "", regex=True).astype(float)
    
    fig, ax = plt.subplots(figsize=(12, 6), dpi=100)
    ax.plot(df["Mês"], df["vendas_numerico"], lw=3, marker="o", color='tab:blue')
    ax.set_title("Total de Vendas", fontsize=18, loc="left")
    ax.set_xlabel("Mês", fontsize=14)
    ax.set_ylabel("Vendas (em milhares de reais)", fontsize=14)
    ax.set_frame_on(False)
    ax.grid(True, color='gray', linestyle="--")
    
    ax.tick_params(axis='both', which='both', length=0)
    plt.ylim(0, df["vendas_numerico"].max() + 100)

    for i, row in df.iterrows():
        ax.annotate(f"R${row['vendas_numerico']:.2f}", xy=(row['Mês'], row['vendas_numerico']), 
                    xytext=(5, 5), textcoords='offset points', fontsize=10)
    
    plt.savefig(filename, dpi=100, bbox_inches='tight', pad_inches=0)
    plt.show()
