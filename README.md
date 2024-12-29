## 📊 Análise de Vendas 2023

Este projeto realiza uma análise abrangente das vendas mensais, lucro por departamento, modos de envio mais utilizados em São Paulo, lucro total, lucro por segmentação de clientes, lucros por estado brasileiro e por produto no ano de 2023. Ele cria gráficos a partir dos dados, exporta os resultados para arquivos Excel e gera um relatório PDF

## Sumário

- [Descrição](#descrição)
- [Pré-requisitos](#pré-requisitos)
- [Instalação](#instalação)
- [Uso](#uso)
- [Funções](#funções)
- [Contribuição](#contribuição)
- [Licença](#licença)
- [Contato](#contato)
- [Dashboard](#dashboard)

## Descrição

Este projeto foi desenvolvido para analisar dados de vendas mensais, lucro por departamento, modos de envio mais utilizados em São Paulo, lucro total, lucro por segmentação de clientes, lucros por estado brasileiro e por produto no ano de 2023. Ele gera gráficos ilustrativos, exporta os dados processados para arquivos Excel e gera um relatório PDF detalhado. O principal objetivo é fornecer visualizações claras e compreensíveis das tendências e padrões encontrados nos dados.


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

2. O script exportará arquivos Excel chamados `tb_distribuicao_lucro_por_regiao.xlsx`, `tb_envio_sp.xlsx`,`tb_lucro_dpt.xlsx`,`tb_lucro_por_produto.xlsx` e `tb_vendas_por_mes.xlsx`, além de salvar os gráficos correspondentes como `Vendas_por_mes.png`, `Lucro_por_Departamento_Anual.png`, `Modos_Envio_São_Paulo.png`, `Lucro_por_regiao_barras.png` e `Lucro_por_produto.png`. Ele também gerará um relatório PDF chamado `Relatório_2023.pdf`.

## Dashboard

![image](https://github.com/user-attachments/assets/da522f90-a324-4774-bad1-e97cc7cadca9)


## Funções

Análise de vendas mensais

Cálculo de lucro por departamento

Identificação dos modos de envio mais utilizados em São Paulo

Cálculo do lucro total

Segmentação de lucros por tipo de cliente

Análise de lucros por estado brasileiro

Análise de lucros por produto no ano de 2023

## Contribuição

Contribuições são bem-vindas! Se você tem sugestões, encontrou um bug ou deseja adicionar uma nova funcionalidade, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto está licenciado sob a Licença MIT. Veja o arquivo LICENSE para mais detalhes.


