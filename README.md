# Decision Tree Classification on the Iris Dataset

## Overview
This project implements a **Decision Tree Classifier** for a **multi-class supervised classification problem** using the **Iris dataset**.  
The focus of this project is not only on model training but also on **controlling overfitting** through **pre-pruning and post-pruning techniques**, optimized using **GridSearchCV**.

---

## Dataset
- **Name:** Iris Dataset  
- **Source:** Scikit-learn built-in dataset  
- **Samples:** 150  
- **Features:**  
  - Sepal Length  
  - Sepal Width  
  - Petal Length  
  - Petal Width  
- **Target Classes:**  
  - Setosa  
  - Versicolor  
  - Virginica  

---

## Model Used
- **Decision Tree Classifier**
  - Splitting Criterion: Gini Index / Entropy
  - Hyperparameters optimized using GridSearchCV

---

## Workflow

1. Load the Iris dataset  
2. Split the dataset into training and testing sets  
3. Initialize the Decision Tree classifier  

### Post-Pruning (Cost Complexity Pruning)
4. Generate effective alpha (`ccp_alpha`) values  
5. Use GridSearchCV to tune post-pruning hyperparameters  
6. Train the post-pruned decision tree model  
7. Evaluate performance on test data  

### Pre-Pruning
4. Define pre-pruning hyperparameters (`max_depth`, `min_samples_split`, `min_samples_leaf`)  
5. Apply GridSearchCV to find optimal pre-pruning values  
6. Train the pre-pruned decision tree model  
7. Evaluate performance on test data  

---

## Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## Visualization
- Confusion matrix visualized using Seaborn  
- Comparative analysis of pre-pruned and post-pruned models  

---

## Technologies Used
- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## Project Structure
├── decision_tree_iris_classification.ipynb

├── README.md

---

## Key Learnings
- Decision Trees are prone to overfitting without pruning
- Pre-pruning controls tree growth during training
- Post-pruning simplifies a fully grown tree using cost complexity pruning
- GridSearchCV helps identify optimal hyperparameters systematically
- Confusion matrices provide deeper insight into class-wise predictions

---

## Author
Nisarg Patel  
Aspiring Data Scientist | Machine Learning Enthusiast

---

## Conclusion
This project demonstrates effective application of **Decision Tree Classification** with **pre-pruning and post-pruning strategies** to improve generalization and interpretability on a standard benchmark dataset.
