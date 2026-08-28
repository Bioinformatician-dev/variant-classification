# 🧬 ClinVar Variant Classification Using Machine Learning

This project tackles the challenge of classifying **clinically conflicting genetic variants** (Benign vs Pathogenic) using supervised **machine learning models** on annotated ClinVar data.

We explore a variety of statistical and ML techniques to understand patterns in mutation consequences, population allele frequencies, and prediction scores (SIFT, PolyPhen, CADD), and use them to build predictive models.



## 🚀 Project Highlights

- ✅ Downloaded and processed the **ClinVar Conflicting Variants** dataset from Kaggle
- 📊 Performed **extensive EDA**: gene frequency, mutation consequence (MC) heatmaps, CADD boxplots, and correlation analysis
- 🔍 Applied **feature engineering** on categorical predictors (SIFT & PolyPhen)
- 🤖 Trained and evaluated 6 ML classifiers:
  - Logistic Regression
  - Random Forest
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)
  - MLP Neural Network
  - Gaussian Naive Bayes
- 📈 Compared model performance using accuracy, precision, recall, F1-score, and confusion matrices



## 🧬 Dataset

- **Source**: [Kaggle - ClinVar Conflicting](https://www.kaggle.com/datasets/kevinarvai/clinvar-conflicting)
- **Size**: ~7K clinically annotated SNVs
- **Key Features**:
  - `CADD_PHRED`: Deleteriousness score
  - `AF_ESP`, `AF_EXAC`, `AF_TGP`: Population allele frequencies
  - `SIFT`, `PolyPhen`: In-silico predictors
  - `MC`: Mutation consequences
  - `CLASS`: Target (0 = Benign, 1 = Pathogenic).



## 📁 Project Structure

```bash
variant-classification/
├── data/
│   └──dataset.py       # Dataset to downlowd and unzip
├── notebooks/
│   └── 01_exploratory_analysis.ipynb  # EDA and data visualization
│   └── 02_model_training.ipynb        # Classifier training and evaluation               
├── results/
│   └── figures/                       # Plots and figures
│       └── model_accuracy.png
├── README.md

```
