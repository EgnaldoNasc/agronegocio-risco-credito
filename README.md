# 🚜 Modelo de Risco de Crédito para Produtores Rurais

Este projeto tem como objetivo desenvolver um modelo de machine learning para prever o risco de crédito de produtores rurais no contexto do agronegócio, utilizando dados simulados. A proposta é oferecer uma solução analítica que possa apoiar instituições financeiras na tomada de decisão de concessão de crédito no setor agropecuário.

---

## 🎯 Objetivos

- Simular um conjunto de dados representando produtores rurais com características típicas do setor agrícola brasileiro;
- Realizar tratamento e limpeza dos dados;
- Aplicar técnicas de engenharia de atributos e análise estatística;
- Treinar modelos supervisionados (classificação) com foco em previsão de inadimplência;
- Avaliar o desempenho dos modelos com métricas robustas (AUC, F1, precisão, recall);
- Apresentar insights acionáveis para diferentes stakeholders;
- Simular cenários de backtest para avaliação prática da solução.

---

## 🧰 Tecnologias Utilizadas

- **Python** 3.10+
- **Pandas**, **NumPy**
- **Scikit-learn**, **XGBoost**
- **Matplotlib**, **Seaborn**
- **SHAP** (para interpretabilidade)
- **Jupyter Notebook**
- **Git** / **GitHub** (versão e colaboração)
- **Streamlit** (dashboard interativo - opcional)

---

## 📁 Estrutura do Projeto

```
risco-credito-produtores-rurais/
├── data/                  # Conjunto de dados simulados
│   ├── raw/               # Dados brutos
│   └── processed/         # Dados limpos
├── notebooks/
│   ├── 01_analise_exploratoria.ipynb
│   ├── 02_modelagem_classificacao.ipynb
│   └── 03_backtest_simulado.ipynb
├── src/                   # Scripts reutilizáveis
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   └── model_training.py
├── reports/
│   ├── apresentacao.pdf   # Slides dos resultados
│   └── metricas_modelo.xlsx
├── requirements.txt
├── README.md
└── streamlit_app.py       # Dashboard (opcional)
```

---

## 📊 Dados Utilizados

Os dados são **sintéticos**, mas foram modelados com base em características reais do setor. Cada registro representa um produtor rural, com variáveis como:

- Área plantada (hectares)
- Tipo de cultivo (milho, soja, cana, etc.)
- Receita estimada da última safra
- Score de crédito anterior
- Histórico de inadimplência
- Presença de garantias
- Região de atuação

---

## 📈 Modelagem Preditiva

Modelos testados:

- Regressão Logística
- Random Forest
- XGBoost

### Métricas de avaliação:
- AUC-ROC
- F1-Score
- Matriz de Confusão
- Curva Precision-Recall

Utilizamos validação cruzada e análise de variáveis explicativas com **SHAP**.

---

## 🔍 Principais Resultados

- Melhor modelo: **XGBoost**
- AUC-ROC: **0.84**
- F1-Score: **0.78**
- Redução de 22% em falsos positivos com abordagem de reclassificação
- Identificação de 5 principais variáveis com maior poder preditivo

---

## 🖥️ Dashboard Interativo (opcional)

Para executar o painel interativo:

```bash
streamlit run streamlit_app.py
```

---

## 📌 Como Executar Localmente

1. Clone este repositório:
```bash
git clone https://github.com/seunome/risco-credito-produtores-rurais.git
cd risco-credito-produtores-rurais
```

2. Instale as dependências:
```bash
pip install -r requirements.txt
```

3. Inicie os notebooks:
```bash
jupyter notebook
```

---

## 🧠 Próximos Passos

- Conectar com bases públicas (IBGE, CONAB) para testes em dados reais;
- Incorporar sazonalidade e clima no modelo;
- Criar API para consumo externo do modelo;
- Melhorar pipeline de produção com MLflow e DVC.

---

## 👨‍💼 Autor

Desenvolvido por [Seu Nome] — Cientista de Dados com experiência em modelagem de risco, análise preditiva e soluções para o agronegócio.  
📧 [seuemail@email.com]  
🔗 [linkedin.com/in/seunome](https://linkedin.com/in/seunome)

---

**Este projeto é fictício para fins de portfólio, mas pode ser adaptado para aplicações reais no setor de crédito agrícola.**

