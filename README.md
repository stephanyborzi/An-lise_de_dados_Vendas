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

