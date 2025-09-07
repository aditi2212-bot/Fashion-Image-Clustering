# 🧥 Fashion-MNIST Classification & Clustering  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1OUGz2DXUXEbcJq64MWQ6OD8RgNseiEO9?usp=sharing)]

##  Introduction  
This project applies **both supervised and unsupervised learning** techniques on the **Fashion-MNIST dataset**, which consists of 70,000 grayscale clothing images (28×28 pixels) across 10 categories (T-shirt, Trouser, Dress, etc.).  

The main objectives are:  
-  Build and evaluate **classification models** (Logistic Regression, Elastic Net).  
-  Perform **unsupervised clustering** using CNN feature extraction + PCA + KMeans.  
-  Compare model performance using **accuracy, precision, recall, F1, ARI, and NMI**.  
-  Provide **visual insights** with bar charts, confusion matrices, and cluster samples.  

---

##  Business Use Case  
Such models can be applied in:  
- **E-commerce**: Automatically grouping clothing items into categories.  
- **Recommendation Systems**: Suggesting similar products to customers.  
- **Data Cleaning**: Detecting mislabeled items in large product catalogs.  

---

##  Methodology  
1. **Data Preprocessing**  
   - Loaded Fashion-MNIST dataset  
   - Converted grayscale images to RGB for CNN  
   - Resized to 96×96 for feature extraction  

2. **Exploratory Data Analysis (EDA)**  
   - Label distribution bar chart  
   - Sample original clothing images  

3. **Models**  
   - Logistic Regression (baseline)  
   - Elastic Net Logistic Regression (regularized, improved accuracy)  
   - CNN + PCA + KMeans (unsupervised clustering)  

4. **Evaluation Metrics**  
   - Accuracy, Precision, Recall, F1 (classification models)  
   - Adjusted Rand Index (ARI), Normalized Mutual Information (NMI) (clustering)  

5. **Visualizations**  
   - Label distribution (UDI analysis)  
   - Cluster distribution bar chart  
   - Confusion matrix heatmap  
   - Cluster sample images with majority label  

---

##  Results  

| Model                          | Score   |
|--------------------------------|---------|
| Logistic Regression (Accuracy) | ~71%    |
| Elastic Net (Accuracy)         | ~75%    |
| CNN + PCA + KMeans (ARI)       | ~0.45–0.50 |
| CNN + PCA + KMeans (NMI)       | ~0.50–0.55 |

- Logistic Regression gave ~71% baseline accuracy  
- Elastic Net improved performance to ~75%  
- CNN + PCA + KMeans formed meaningful clusters (e.g., trousers grouped together)  

---

##  Requirements  
- Python 3.x  
- TensorFlow  
- scikit-learn  
- matplotlib  
- seaborn  
- pandas  


