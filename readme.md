# 🌍 Projeto de Clusterização — Índice de Desenvolvimento de Países

Este projeto foi desenvolvido como parte do módulo de **Aprendizado Não Supervisionado (Clusterização)** do curso de Pós-Graduação em Inteligência Artificial do Instituto Infnet (MIT em IA).

O objetivo é aplicar técnicas de **clusterização (K-Means e Hierárquica)** para agrupar países com base em indicadores socioeconômicos e de saúde, identificando padrões de desenvolvimento.

---

## 🧠 Objetivos do Projeto

1. **Explorar os dados** socioeconômicos e de saúde  
2. **Pré-processar os dados** (limpeza, escala, inspeção)  
3. Aplicar **K-Means** e **Clusterização Hierárquica**  
4. **Comparar resultados** entre os métodos  
5. Avaliar **sensibilidade a outliers** e robustez do **DBSCAN**

---

## 📦 Dataset

**Fonte:**  
[Kaggle — Unsupervised Learning on Country Data](https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data)

---

## 📁 Estrutura do Projeto

```bash
.
├── data/                    # Dados utilizados (não versionados)
│   └── Country-data.csv
├── notebooks/
│   └── clusterizacao_paises.ipynb
├── outputs/
│   ├── histogramas/
│   ├── boxplots/
│   └── pca_clusters.png
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 🧩 Etapas Desenvolvidas

### ✅ Pré-processamento
- Tratamento de dados ausentes  
- Padronização com **StandardScaler**  
- Geração de histogramas e boxplots  
- Análise de correlação entre variáveis  

### ✅ Clusterização
- Aplicação do **K-Means** com K=3  
- **Clusterização Hierárquica** com método *Ward*  
- Identificação dos **medóides** (países representativos)  

### ✅ Comparação
- Tabela de contingência entre métodos  
- Cálculo do **Adjusted Rand Score**  
- Visualização via **PCA**

---

## 🧪 Tecnologias Utilizadas

- Python 3.10+  
- Pandas  
- NumPy  
- Scikit-Learn  
- SciPy  
- Matplotlib / Seaborn  

---

## ▶️ Como Executar

```bash
# Criar ambiente virtual
python -m venv .venv

# Ativar ambiente
source .venv/bin/activate        # Mac/Linux
.venv\Scripts\activate           # Windows

# Instalar dependências
pip install -r requirements.txt

# Executar notebook
jupyter notebook notebooks/clusterizacao_paises.ipynb
```

---

## ✨ Resultados

- Identificação de **3 perfis principais de desenvolvimento**:
  - Países desenvolvidos  
  - Países em desenvolvimento  
  - Países com baixo IDH  
- Países representativos (medóides) de cada cluster  
- Gráfico PCA comparando **K-Means vs Hierárquico**  
- Dendrograma e análise comparativa de métodos  
