# Hybrid Stress Detection in Social Media: A Psycholinguistic Approach

## 📌 Project Overview
This project focuses on identifying psychological stress in social media posts using the **Dreaddit** dataset. Moving beyond simple text classification, this study implements a **Hybrid Meta-Data Model** that integrates lexical features (TF-IDF) with structural psycholinguistic markers (LIWC/DAL). 

The final model is optimized for high-sensitivity triage, specifically designed for potential deployment in university student communities like **r/nus**.

## 📊 Key Results
* **F1-Score:** 0.7842 (A significant improvement over the 0.72 text-only baseline)
* **Recall (Sensitivity):** 0.8618 — Optimized to minimize False Negatives in clinical contexts.
* **Precision:** 0.7195

## 🛠️ Technical Stack
* **Language:** Python 3.10+
* **Modeling:** Logistic Regression, Random Forest (for feature selection)
* **NLP:** Scikit-Learn (TF-IDF Vectorization, Pipelines, ColumnTransformers)
* **Interpretability:** SHAP (SHapley Additive exPlanations)
* **Visualization:** Matplotlib, Seaborn

## 📂 Project Structure
* `assignment2.ipynb`: The complete end-to-end pipeline (Preprocessing -> Feature Engineering -> Model Selection -> Evaluation).
* `requirements.txt`: List of Python dependencies required to replicate the environment.
* `data/`: Directory containing `dreaddit-train.csv` and `dreaddit-test.csv`.

---

## ⚙️ How to Run the Project

### 1. Clone the Repository
First, clone the repository to your local machine and navigate into the project directory:
```bash
git clone git@github.com:reanosy26/DSA4262.git
cd DSA4262
cd assignment_2
```

### 2. Environment Setup
It is highly recommended to use a virtual environment to avoid library conflicts:
```bash
# Create a virtual environment
python -m venv venv

# Activate it
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

# Install required libraries
pip install -r requirements.txt
```