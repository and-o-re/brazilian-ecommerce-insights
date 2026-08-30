# 📊 Relatório E-Commerce no Brasil: Análise Regional de Investimento

## 🎯 Sobre o Projeto
Este projeto é um trabalho de pesquisa e análise de dados desenvolvido para o Tech Challenge da Fase 1 da Pós Tech em Data Analytics da FIAP. 

O estudo realiza uma análise multidimensional do **Brazilian E-Commerce Public Dataset by Olist**. O objetivo central é responder à seguinte pergunta de negócio: **Onde o investimento deve ser priorizado, considerando o potencial financeiro e a saúde operacional de cada Estado?**

## 🛠️ Tecnologias e Ferramentas
* **Linguagens e Bancos:** Python, SQL (DuckDB)
* **Manipulação de Dados:** Pandas, NumPy, Pathlib
* **Visualização:** Matplotlib, Seaborn
* **Machine Learning & Pré-processamento:** Scikit-learn (MinMaxScaler)
* **Ambiente de Desenvolvimento:** Google Colab

## 🧠 Metodologia
A análise seguiu um pipeline robusto de preparação, exploração e consolidação regional dos dados. Para definir as prioridades de investimento, foram criados indicadores compostos:
* **Score Financeiro:** Calculado a partir da quantidade de pedidos e da receita gerada por UF.
* **Score Operacional:** Calculado a partir da taxa de atrasos e do impacto do frete sobre o preço do produto.
* **Score de Oportunidade:** Consolidação dos fatores financeiros (60%) e operacionais (40%).
* **Normalização:** Todos os dados foram normalizados utilizando a técnica MinMaxScaler para posicionar os valores proporcionalmente em scores de 0 a 100.

## 📈 Principais Resultados (Matriz de Priorização)
A matriz classificou os estados brasileiros em cinco categorias de ação estratégica:

* **Consolidar (SP):** São Paulo obteve o maior score de Oportunidade (97). O estado concentra a maior parte dos pedidos e possui a menor barreira logística do dataset. Além disso, 71,3% dos vendedores estão concentrados nesta região.
* **Expandir (MG, RJ, PR, RS, DF, SC, GO, MT, ES):** Estas regiões apresentam uma operação logística saudável, com scores operacionais variando entre 62 e 92. O risco de expansão é baixo, justificando investimentos em campanhas de marketing ou captação de vendedores locais.
* **Corrigir antes de Expandir (BA, PE, PA, CE):** Existe demanda comercial evidente, porém o score operacional está abaixo da mediana (44 a 54). Os altos índices de atraso e o frete elevado comprometem a experiência do consumidor. É necessário investir em melhorias logísticas antes de focar em aquisição.
* **Desenvolver (AP, AM, MS, AC):** Estados com demanda comercial muito baixa, porém sem gargalos operacionais graves aparentes.
* **Monitorar (RN, PB, TO, SE, PI, RR, MA, AL, RO):** Regiões com volume comercial e maturidade operacional ainda em desenvolvimento. No Amazonas, por exemplo, o tempo mediano de entrega chega a 26 dias, evidenciando gargalos. Alagoas lidera os problemas de pontualidade, com 24,12% dos pedidos atrasados.

## 👥 Equipe de Pesquisa
* André Carlos Soares de Souza
* Anne Pimentel Alexandre da Silva
* Daniella de Castro Alves
* Ewerton Pereira Reis

## 📚 Referências
* OLIST. *Brazilian E-Commerce Public Dataset by Olist*. Kaggle, 2018.
