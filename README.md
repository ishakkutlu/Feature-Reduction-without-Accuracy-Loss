# Feature Reduction without Accuracy Loss

## 🔍 Overview 

This project explores **feature reduction and model interpretability** in a controlled classification task.  
Using a smartphone price dataset, the experiment shows that even with **85% fewer features (20 → 3)**, model performance remains nearly unchanged **(~91% accuracy)**.  
The workflow illustrates how to identify the most informative variables and remove redundant dimensions without losing predictive power.   

---

## ⚙️ Methodology  

- **Task:** Multiclass price-category classification  
- **Model:** k-Nearest Neighbors (k-NN)  
- **Feature Selection & Extraction:** Statistical filtering and dimensionality reduction  
- **Evaluation:** Baseline (all features) vs. reduced model (3 key predictors)  
- **Key Features Retained:** RAM, battery_power, sc_solution (derived from px_height and px_width)  

---

## 📊 Results  

| Model Version | # Features | Accuracy | Reduction |  
| ------------- | ---------- | -------- | --------- |  
| Baseline      | 20         | 0.91     | —         |  
| Reduced       | 3          | 0.91     | **−85%**  |  

Despite the 85% reduction in dimensionality, the classification accuracy remained stable, demonstrating the model’s **robustness** and the power of **informed feature selection**.  

---

## 💡 Insights

- Redundant and correlated features can inflate model complexity without improving results.  
- Intelligent selection of minimal yet informative variables improves efficiency and interpretability.  
- Compact models generalize better, train faster, and simplify deployment pipelines.  

---

## 🧰 Tools  

Python · Pandas · NumPy · Scikit-learn · Matplotlib · Seaborn

---
 
## 📂 Project File  

The notebook is stored in the [`/notebook`](./notebook) folder. 

Fully reproducible on Kaggle:  
[View Notebook](https://www.kaggle.com/code/shakkutlu/feature-reduction-without-accuracy-loss)  
