Tech Challenge Fase 2 - Classificação da qualidade de vinhos com Machine Learning
# 🍷 Wine Quality Classification

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)
![FIAP](https://img.shields.io/badge/FIAP-Tech%20Challenge-red)

Projeto desenvolvido como parte do **Tech Challenge – Fase 2 (FIAP)** com o objetivo de construir e avaliar modelos de Machine Learning capazes de classificar vinhos em duas categorias de qualidade a partir de suas características físico-químicas.

---

# 📖 Sobre o Projeto

Este projeto contempla todas as etapas de um pipeline de Machine Learning supervisionado, incluindo análise exploratória dos dados (EDA), pré-processamento, engenharia de atributos, treinamento, avaliação e comparação de modelos de classificação.

Foram desenvolvidos dois algoritmos de Machine Learning — **Logistic Regression** e **Random Forest** — com o objetivo de identificar vinhos de alta qualidade a partir de variáveis físico-químicas.

---

# 🎯 Objetivo

Classificar vinhos em duas categorias de qualidade.

| Qualidade Original | Classe |
|-------------------|--------|
| ≥ 7 | Alta qualidade (1) |
| < 7 | Baixa/Média qualidade (0) |

A variável original **quality** foi transformada em uma variável binária denominada **high_quality**, permitindo tratar o problema como uma tarefa de classificação supervisionada.

---

# 📊 Dataset

Foi utilizada a base **WineQT**, composta por:

- **1.143 registros**
- **13 atributos físico-químicos**

Entre as variáveis disponíveis destacam-se:

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol

---

# 🛠 Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

# 🔎 Pipeline do Projeto

O desenvolvimento foi dividido nas seguintes etapas:

1. Análise Exploratória dos Dados (EDA)
2. Visualização estatística
3. Criação da variável alvo (Classificação Binária)
4. Pré-processamento dos dados
5. Separação em conjuntos de treino e teste
6. Padronização das variáveis utilizando StandardScaler
7. Treinamento dos modelos de Machine Learning
8. Avaliação utilizando Accuracy, Precision, Recall, F1-Score e AUC
9. Interpretação das variáveis mais relevantes

---

# 📈 Resultados

| Métrica | Logistic Regression | Random Forest |
|---------|--------------------:|--------------:|
| Accuracy | 90,83% | **91,70%** |
| Precision | 65,22% | **69,57%** |
| Recall | 53,57% | **57,14%** |
| F1-Score | 58,82% | **62,75%** |
| AUC | 90,10% | **95,91%** |

---

# 🏆 Modelo Selecionado

O modelo **Random Forest** apresentou o melhor desempenho geral, obtendo maiores valores para Accuracy, Precision, F1-Score e AUC.

Além do melhor desempenho preditivo, o modelo permitiu identificar as variáveis mais importantes para a classificação dos vinhos, destacando principalmente:

- Alcohol
- Sulphates
- Volatile Acidity

---

# 💡 Principais Insights

- O conjunto de dados apresentou desbalanceamento entre as classes.
- O teor alcoólico foi a variável mais importante para o modelo Random Forest.
- A utilização conjunta de Accuracy, Precision, Recall, F1-Score e AUC proporcionou uma avaliação mais completa dos modelos.
- A análise de importância das variáveis reforçou o entendimento dos fatores físico-químicos mais relevantes para a classificação da qualidade dos vinhos.
- O modelo Random Forest apresentou desempenho superior ao da Logistic Regression para o problema proposto.

---

# 📁 Estrutura do Repositório

```text
wine-quality-classification/

├── data/
│   └── WineQT.csv
│
├── notebooks/
│   └── Tech_Challenge_Fase_2_FIAP.ipynb
│
├── resultados/
│   ├── Apresentacao_Executiva.pdf
│   └── comparacao_modelos.csv
│
├── requirements.txt
│
└── README.md
```

---

# ▶️ Como Executar

```bash
git clone https://github.com/vicagt/wine-quality-classification.git

cd wine-quality-classification

pip install -r requirements.txt

jupyter notebook
```

---

# 👨‍💻 Autor

**Victor Schiavone**,
**Juliana Bahia**,
**Guilherme Ledier**,
**Gisele Domingues**,
**Alexandre Amaro**


Projeto desenvolvido como parte do **Tech Challenge – Fase 2** da Pós-Tech em Data Analytics da **FIAP**.

---

# 📄 Licença

Projeto desenvolvido exclusivamente para fins acadêmicos como parte do Tech Challenge – Fase 2 da FIAP, podendo também ser utilizado como material de portfólio.
