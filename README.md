# Support-Vector-Machines-SVM-
This task focuses on using Support Vector Machines (SVM) for binary classification using both **linear** and **RBF (non-linear)** kernels. The dataset used is the **Breast Cancer Dataset** from Kaggle.

## Objectives
- Understand the concept of SVMs and the kernel trick
- Train SVMs with both linear and RBF kernels
- Visualize decision boundaries in 2D using PCA
- Perform hyperparameter tuning using GridSearchCV
- Evaluate the model using cross-validation

---

## Dataset
- **Name**: Breast Cancer Dataset
- **Link**: [Click to open on Kaggle](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)
- **Target Variable**: Diagnosis (`M` for malignant, `B` for benign)
- **Features**: Mean values of various cell nucleus features

---

## 🧪 Libraries Used
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

## Steps Performed

### 1. Data Preprocessing
- Loaded CSV dataset
- Converted categorical target variable into binary (0 and 1)
- Scaled feature values using `StandardScaler`
- Split into training and testing sets

### 2. Model Training
- Trained two SVM classifiers:
  - SVM with Linear Kernel
  - SVM with RBF Kernel

### 3. Visualization
- Used PCA to reduce features to 2D
- Plotted decision boundary of SVM

### 4. Hyperparameter Tuning
- Used `GridSearchCV` to find optimal values of:
  - `C` (regularization parameter)
  - `gamma` (for RBF kernel)

### 5. Cross-Validation
- Applied 5-fold cross-validation
- Evaluated average accuracy

---

## Results

| Model           | Accuracy (Test Data) |
|----------------|----------------------|
| SVM (Linear)   | ~97%                 |
| SVM (RBF)      | ~98%                 |

