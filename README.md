# 💊 Real-World Health Signal Analysis

**Problem:**  
What are the most commonly reported side effects for top drugs, and how do sentiments about these drugs vary over time?

## 🔍 Scope

**Target drugs:**  
Top 10 most-reviewed drugs from user submissions.

**Key questions:**
- What side effects do people frequently mention in their reviews?
- How does public sentiment shift across time and age groups?

## 📦 Datasets

1. [Drug Reviews - KUC Hackathon 2018](https://www.kaggle.com/datasets/jessicali9530/kuc-hackathon-winter-2018)
2. [Drug Review Dataset (Detailed)](https://www.kaggle.com/datasets/mohamedabdelwahabali/drugreview)
3. [SIDER Side Effect Resource (MedDRA)](http://sideeffects.embl.de/)

## 🧠 Methodology

### 🔹 Data Preparation
- Merged multiple review datasets
- Cleaned text, filtered by drug mentions

### 🔹 Sentiment Analysis
- Used [VADER](https://github.com/cjhutto/vaderSentiment) to classify review sentiment (positive, neutral, negative)
- Smoothed sentiment over time for visual trends

### 🔹 Side Effect Extraction
- Loaded side effect list from SIDER (MedDRA terms)
- Used phrase matching to detect mentions in user reviews

### 🔹 Visualizations
- Line plots of sentiment over time per drug
- Bar charts of most reported side effects

## 📊 Sample Insights

>

## 🛠️ Requirements

```bash
pip install -r requirements.txt
```

## 📁 Repository Structure

- `data/`: Raw and cleaned datasets
- `notebooks/`: Analysis steps in Jupyter notebooks
- `outputs/`: Final results and visualizations
- `utils/`: Helper functions/scripts

## 📌 Future Work

- Use SciSpacy/MedSpaCy for more advanced NER
- Correlate side effects with sentiment trends
- Expand to include dosage-related effects

## 👩‍🔬 Author

**Aishwarya** – Data Tech Analyst  
*Exploring public perception of medicines through real-world reviews.*
