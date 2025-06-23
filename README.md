# Customer Segmentation with Unsupervised Learning  
*Final Project – Unsupervised Learning Specialization*

All figures (EDA histograms, PCA plot, cluster scatter) are inside the notebook.

## Overview  
Wholesale distributors often struggle to tailor promotions to customers who buy very different mixes of products.  
This project clusters **440 wholesale customers** by their annual spend across six product categories and reveals two clear, actionable segments (“Bulk / High-Value” vs “Light Buyers”).

* **Dataset** – [UCI Wholesale customers](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers)  
* **Tech** – Python, pandas, scikit-learn, seaborn, matplotlib  
* **Key metric** – Silhouette score (best *k* = 2, score ≈ 0.29)  
* **Outcome** – Cluster profiles expose buyers who warrant volume discounts vs loyalty incentives.

---

## Repository contents  

| File | Purpose |
|------|---------|
| `unsupervised_customer_segmentation.ipynb` | Full notebook: EDA → PCA → K-Means & Ward clustering → conclusions |
| `README.md` | You’re reading it |

*(No separate requirements file—the notebook prints library versions inside the **Reproducibility** cell so peers can install manually.)*

---

## Quick-start  

    # 1. Clone the repo
    git clone https://github.com/<YOUR-USERNAME>/unsupervised-customer-segmentation.git
    cd unsupervised-customer-segmentation

    # 2. Install core dependencies
    pip install pandas numpy scikit-learn seaborn matplotlib scipy

    # 3. Launch the notebook
    jupyter notebook unsupervised_customer_segmentation.ipynb

All models use `random_state = 42`, so you’ll reproduce the exact clusters and plots.

---

## Results snapshot  

| Cluster | Fresh | Milk | Grocery | Frozen | Detergents & Paper | Delicassen |
|---------|------:|-----:|--------:|-------:|-------------------:|-----------:|
| **0 – Light Buyers** | 7 100 | 3 500 | 5 800 | 1 700 | 1 000 | 1 100 |
| **1 – Bulk Buyers**  | 15 100 | 7 800 | 14 000 | 3 900 | 6 100 | 2 100 |

> *Cluster 1 spends roughly **2 ×** across all categories and is an ideal candidate for volume-based incentives.*

---

## Reproducibility  
Run the **Environment & Dependencies** cell at the end of the notebook to print the exact library versions (pandas 2.x, scikit-learn 1.3, etc.).  
Any Python ≥ 3.8 environment with those libs will work.

---

> Dataset provided by the UCI Machine Learning Repository. Free for research and educational use.
