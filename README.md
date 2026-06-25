# DataView - Análise Exploratória de Vendas

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-green?style=flat&logo=pandas)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange?style=flat&logo=jupyter)

##  Sobre o Projeto

O **DataView PY** é um projeto de **Análise Exploratória de Dados (EDA)** desenvolvido em Python, simulando o dia a dia de um Analista de Dados Júnior. O sistema recebe um dataset de vendas **intencionalmente bagunçado** (com dados nulos, datas inválidas e textos sujos), realiza uma limpeza completa, cria novas métricas, gera gráficos profissionais e exporta relatórios prontos para a tomada de decisão.

> **Objetivo principal:** Transformar dados "sujos" em insights valiosos para o time de negócios, utilizando apenas código Python e bibliotecas de análise.

---

## Sobre o que é analise?

| Análise | Descrição |
| :--- | :--- |
| ** Receita e Volume** | Vendas totais e quantidade de itens vendidos por mês e trimestre. |
| ** Top Produtos** | Ranking dos 5 produtos e categorias que mais geraram receita. |
| ** Desempenho Regional** | Comparação de receita e ticket médio por região do país. |
| ** Segmentação de Clientes** | Classificação dos clientes em **Bronze**, **Prata** e **Ouro** com base no total gasto. |
| ** Tratamento de Outliers** | Comparação entre duas versões da base: **v1** (com outliers mantidos) e **v2** (com outliers tratados via IQR). |
| ** Exportação** | Geração de relatórios em formatos **CSV** (tabelas) e **JSON** (estatísticas gerais). |
| ** Visualização** | Criação de gráficos de linha, barras e boxplot exportados em alta qualidade (**PNG**). |

---

## Conceitos Aplicados

Este projeto foi desenvolvido para demonstrar domínio prático das seguintes ferramentas e conceitos de **Ciência de Dados** e **Python**:

- **Lógica de Programação:** Variáveis, tipos de dados, operadores, estruturas condicionais (`if/elif/else`) e loops (`for`).
- **Funções:** Criação de funções com parâmetros, retornos, **funções lambda** e reutilização de código.
- **Leitura e Escrita:** Manipulação de arquivos nos formatos **CSV** e **JSON**.
- **Manipulação de Datas:** Extração de mês, trimestre e ano utilizando o módulo `datetime`.
- **Expressões Regulares (`re`):** Limpeza avançada de textos, removendo espaços extras e normalizando strings.
- **Pandas:** Manipulação de DataFrames, tratamento de valores nulos, filtros booleanos, agrupamentos (`groupby`) e transformações.
- **NumPy:** Operações vetorizadas, broadcasting, cálculos estatísticos (média, mediana, percentis) e filtros com Boolean Indexing.
- **Detecção de Outliers:** Aplicação do método estatístico **IQR (Intervalo Interquartil)** para detecção e remoção de dados anômalos.
- **Visualização de Dados:** Construção de gráficos informativos com **Matplotlib** e **Seaborn**, incluindo personalização de títulos, rótulos e exportação para PNG.
- **Versionamento:** Boas práticas de commits e organização do repositório no **GitHub**.

---

## Estrutura do Projeto

A organização das pastas segue o padrão de um pipeline de dados profissional:

```text
projeto-data-view/
│
├── data/                         # Todos os dados do projeto
│   ├── final/                      # Dataset bruto (gerado sinteticamente)
│   ├── processed/
│   │   ├── v1_com_outliers/      # Dados limpos, mas com valores extremos mantidos
│   │   └── v2_outliers_tratado/  # Dados limpos e com outliers removidos
│   └── final/                    # Dataset final enriquecido (escolhido para análise)
│
├── notebooks/
│   └── dataview.ipynb            # Notebook principal com todo o código e execuções
│
├── outputs/                       # Resultados finais gerados pelo sistema
│   ├── graficos/                  # Imagens PNG geradas (receita, produtos, região)
│   ├── metricas_por_mes.csv       # Resumo das vendas mês a mês
│   ├── segmentacao_clientes.csv   # Tabela com a classificação dos clientes
│   └── estatisticas_gerais.json   # Estatísticas numéricas em formato JSON
│
├── README.md                      # Documentação oficial do projeto
└── .gitignore                     # Arquivos que não devem subir para o GitHub


 Como Executar o Projeto
Você pode executar o sistema de duas maneiras: Online (recomendado) ou Localmente.

 Opção 1: No Google Colab (Recomendado)
O Google Colab já possui todas as bibliotecas instaladas, não exigindo configuração no seu computador.

Acesse o site: colab.research.google.com

Faça o upload do arquivo dataview.ipynb.

Execute as células na ordem (de cima para baixo) clicando no botão "Play" de cada uma.

 Opção 2: Localmente com VS Code ou Jupyter
Se preferir rodar no seu computador, siga os passos abaixo:

Instale o Python 3.10+ e o editor VS Code.

Instale as dependências necessárias. Abra o terminal e execute:
pip install pandas numpy matplotlib seaborn

Abra o arquivo dataview.ipynb no VS Code e execute as células uma a uma.

 Vídeo de Demonstração
Para entender melhor o funcionamento do projeto na prática, assista ao vídeo explicativo gravado pelo desenvolvedor.

[https://drive.google.com/file/d/1oKGPduxuBqLFGgdyeW40v5D6xSVUHlcS/view?usp=drive_link]

 Observações Finais
A versão final utilizada para as análises e relatórios foi a v2 (com tratamento de outliers), garantindo dados mais consistentes para a tomada de decisão.

##  Ferramentas Utilizadas

* **Linguagem:** Python 3.10+
* **Ambiente de Desenvolvimento:** Google Colab
* **Bibliotecas de Dados:** Pandas, NumPy
* **Bibliotecas de Visualização:** Matplotlib, Seaborn
* **Módulos Nativos Python:** `os`, `re` (Expressões Regulares), `datetime`, `random`, `json`
* **Versionamento de Código:** Git e GitHub



Desenvolvido por: Nivaldo Marinho
Curso: Inteligência Artificial para Análise Preditiva
Data: Junho de 2026



