# Análise da Desigualdade Racial na Desocupação Juvenil (2020-2024)

Repositório contendo o código-fonte e a memória de cálculo do Projeto de Pesquisa Simplificado submetido à Chamada Pública IPEA/PIPA nº 055/2025.

## 📄 Conteúdo do Repositório

* **[`analise_desocupacao_pnad.ipynb`](./analise_desocupacao_pnad.ipynb)**: Jupyter Notebook com o código completo, incluindo:
    1.  Rotina de validação de integridade dos 20 arquivos `.txt` da PNAD.
    2.  Definição do layout posicional (`COLSPECS`).
    3.  Processamento, filtragem e cálculo ponderado das taxas.
* **[`analise_desocupacao_pnad.pdf`](./analise_desocupacao_pnad.pdf)**: Versão estática do notebook para visualização rápida dos resultados e gráficos.

## 🛠️ Metodologia Técnica

O projeto utiliza microdados trimestrais da PNAD Contínua (IBGE). Devido à natureza do formato de largura fixa (*Fixed-Width File*), foi desenvolvida uma rotina de leitura posicional validada empiricamente para garantir a extração correta das variáveis de interesse:
* **Filtro de Escopo:** Jovens (18-24 anos) na Força de Trabalho.
* **Ponderação:** Utilização do peso calibrado (`V1028`) para expansão da amostra.

## 🚀 Como Executar

Para reproduzir a análise:
1.  Baixe os microdados trimestrais (2020-2024) no site do IBGE.
2.  Instale as dependências: `pandas`, `numpy`, `matplotlib`, `seaborn`.
3.  Execute o notebook na mesma pasta dos arquivos `.txt`.

---
*Autor: José Arthur P. Alves*
