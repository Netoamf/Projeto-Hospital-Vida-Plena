# Projeto Hospital Vida Plena - Análise de Dados 🏥📊

Este projeto faz parte da **Carreira de Análise de Dados da Alura**. O principal objetivo é realizar a extração, limpeza (ETL) e análise de base de dados hospitalares fictícios do "Hospital Vida Plena", e em seguida construir um dashboard relacional e interativo para suporte à tomada de decisões estratégicas.

## 🎯 Objetivo do Projeto
Analisar a distribuição, status e ocupação de leitos hospitalares, traçar o perfil dos pacientes e acompanhar as movimentações e internações. Os dados refinados servem como base para a criação de painéis visuais focados em gestão em saúde.

## 🛠️ Tecnologias e Ferramentas
* **Python**: Responsável pela extração, tratamento (ETL) e análise exploratória (EDA).
  * **Bibliotecas**: `pandas`, `matplotlib`, `seaborn`
* **Jupyter Notebook**: Ambiente de execução dos códigos em Python.
* **Microsoft Power BI**: Ferramenta de Business Intelligence utilizada para criação dos dashboards interativos.
* **Microsoft Excel / CSV**: Formatos utilizados para os dados brutos e armazenar as tabelas tratadas.

## 📁 Estrutura de Arquivos

* bases brutas:
  * `eventos_movimentacao.csv`, `leitos.xlsx`, `pacientes.xlsx`: Bases de dados iniciais.
* **`Script_Analysis__.ipynb`**: Notebook responsável por:
  * Renomeação e padronização de colunas.
  * Tratamento de valores temporais (`datetime`) e nulos (`NaN`).
  * Criação de novas colunas categóricas (como Classificação de Idade: Menor de idade, Adulto e Melhor idade).
  * Exploração e visualização elementar de distribuição de Setores e Status de Leitos.
* bases tratadas:
  * `Dados_Tratados.xlsx`, `Leitos_Tratados_Pandas.xlsx`, `Pacientes_Tratados_Pandas.xlsx`: Dados gerados pelo notebook, otimizados para consumo no software de BI.
* **Power BI**:
  * `Analise_HospitalVidaPlena.pbix`: Arquivo completo contendo os relatórios em Power BI.
  * `Modelo_Telas/`: Pasta que contém os templates visuais, capturas de tela do dashboard (`Modelo1.png`, `Modelo2.png`, `Modelo3.png`) e arquivo de tema (`tema_corp_curso.json`).

## 📈 Etapas da Análise

1. **Entendimento dos Dados**: Compreensão das tabelas de leitos, movimentações e detalhamento dos pacientes.
2. **Transformação (ETL)**: Scripts em Python para organizar o esquema e padronizar os dados que alimentariam o modelo.
3. **Análise Exploratória (EDA)**: Uso de gráficos de barra (via relatórios de contagem com seaborn) para medir a disponibilidade de leitos e setores mais demandados.
4. **Construção de Dashboards**: Configuração de tema e montagem de visualizações avançadas (filtros, cartões, totais) usando o Power BI.

## 👀 Como Executar

1. Para ver a etapa de limpeza e tratamento de dados, abra o arquivo `Script_Analysis__.ipynb` com o Jupyter Notebook, JupyterLab ou VS Code e execute as células. *(É necessário ter o pacote `pandas`, `matplotlib`, `seaborn` e suporte ao pacote `openpyxl` na sua máquina local).*
2. Para explorar os relatórios visuais e indicadores, abra o arquivo `Analise_HospitalVidaPlena.pbix` no Microsoft Power BI Desktop.
3. Para pré-visualizar as soluções de layout e telas prontas, verifique as imagens dentro da pasta `Modelo_Telas`.

---
*Projeto desenvolvido como portfólio para a Carreira de Análise de Dados da Alura.*
