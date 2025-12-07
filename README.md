# 🚢 Titanic - Machine Learning from Disaster

A clean, modular machine learning project built locally using **Python 3.12**, **VS Code**, and **GitHub**, using the classic Kaggle Titanic dataset.  
This repository is structured for reproducibility, extendability, and experimentation with different ML models.

## 📁 Project Structure

```
titanic-ml-project/
│
├── .venv/                     # Local virtual environment (not tracked in Git)
│
├── data/
│   └── raw/                   # Kaggle dataset (ignored by Git)
│       ├── train.csv
│       ├── test.csv
│       └── gender_submission.csv
│
├── files_provided_to_ai/      # Reference PDFs used to guide model design
│
├── notebooks/
│   └── eda.ipynb              # Exploratory data analysis notebook
│
├── src/                       # Source code for the ML pipeline
│
├── .gitignore
├── README.md
└── requirements.txt
```

## 🔧 Environment Setup

This project uses **Python 3.12.10** and a local virtual environment.

### 1. Create the virtual environment

```powershell
py -3.12 -m venv .venv
```

### 2. Activate it

```powershell
.venv\Scripts\activate
```

### 3. Install dependencies

```powershell
pip install -r requirements.txt
```

### 4. Select interpreter in VS Code

Open:

**Ctrl + Shift + P → "Python: Select Interpreter" → `.venv/Scripts/python.exe`**

## 📊 Data

The dataset comes from the Kaggle competition:  
**Titanic - Machine Learning from Disaster**

It includes:  
- `train.csv` — training data with labels  
- `test.csv` — evaluation data  
- `gender_submission.csv` — example submission  

You must download the dataset manually from Kaggle and place it into:

```
data/raw/
```

## 🚀 Usage

### Run EDA  
Open the notebook:

```
notebooks/eda.ipynb
```

### Train a model (coming soon)

Run:

```bash
python src/train_model.py
```

### Generate predictions

```bash
python src/predict.py
```

A `submission.csv` file will be created, ready to upload to Kaggle.

## 🏆 Kaggle Competition Info

Kaggle Competition Page:  
https://www.kaggle.com/c/titanic

Goal: Predict which passengers survived the Titanic disaster.  
Metric: **Accuracy** (percentage of correct predictions).

## 📌 Next Steps (Roadmap)

- Implement modular data preprocessing  
- Add feature engineering (Title extraction, Family size, Deck, Ticket groups)  
- Add GBDT models: CatBoost, LightGBM, XGBoost  
- Add cross-validation pipeline  
- Add Optuna for hyperparameter search  
- Add stacking/ensembling  
- Add agent-driven feature exploration (ChatGPT workflows)

## 📜 License

This project follows Kaggle’s competition rules.  
Dataset © Kaggle (subject to competition terms).

## ✨ Author

Created in 2025 as part of a full local ML workflow setup (VS Code + GitHub + ChatGPT Plus).