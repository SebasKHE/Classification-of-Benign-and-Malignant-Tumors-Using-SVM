# Classification-of-Benign-and-Malignant-Tumors-Using-SVM
## **Project Description**  
This project implements a binary classification model using the **Support Vector Machine (SVM)** algorithm to predict whether a tumor is benign or malignant. Based on a medical dataset, the model analyzes specific tumor characteristics to provide accurate and reliable predictions, supporting medical diagnostics.

## **Dataset Structure**  
The dataset includes the following features:  

| **Feature**       | **Description**                                                                        |
|--------------------|----------------------------------------------------------------------------------------|
| `ID`              | Unique identifier for each sample.                                                     |
| `Clump`           | Thickness of cell clumps.                                                              |
| `UnifSize`        | Uniformity of cell size.                                                               |
| `UnifShape`       | Uniformity of cell shape.                                                              |
| `MargAdh`         | Marginal adhesion of cells.                                                            |
| `SingEpiSize`     | Size of single epithelial cells.                                                       |
| `BareNuc`         | Presence of bare nuclei.                                                               |
| `BlandChrom`      | Texture of chromatin.                                                                  |
| `NormNucl`        | Shape of normal nuclei.                                                                |
| `Mit`             | Number of mitoses observed.                                                            |
| `Class`           | Target variable: **2** (Benign) or **4** (Malignant).                                  |

### **Dataset Sample**  
| ID       | Clump | UnifSize | UnifShape | MargAdh | SingEpiSize | BareNuc | BlandChrom | NormNucl | Mit | Class |
|----------|-------|----------|-----------|---------|-------------|---------|------------|----------|-----|-------|
| 1000025  | 5     | 1        | 1         | 1       | 2           | 1       | 3          | 1        | 1   | 2     |
| 1002945  | 5     | 4        | 4         | 5       | 7           | 10      | 3          | 2        | 1   | 2     |
| 1015425  | 3     | 1        | 1         | 1       | 2           | 2       | 3          | 1        | 1   | 2     |
| 1016277  | 6     | 8        | 8         | 1       | 3           | 4       | 3          | 7        | 1   | 2     |
| 1017023  | 4     | 1        | 1         | 3       | 2           | 1       | 3          | 1        | 1   | 2     |

The `Class` attribute is the target variable indicating whether the tumor is benign (2) or malignant (4).

## **Model Results**  
The SVM model achieved the following performance metrics on the test dataset:  

| Metric           | Class 2 (Benign) | Class 4 (Malignant) | Macro Average | Weighted Average |
|-------------------|------------------|---------------------|---------------|-------------------|
| **Precision**     | 1.00             | 0.90                | 0.95          | 0.97              |
| **Recall**        | 0.94             | 1.00                | 0.97          | 0.96              |
| **F1-Score**      | 0.97             | 0.95                | 0.96          | 0.96              |

- **Overall Accuracy:** 96%  

## **Technologies and Tools Used**  
- **Programming Language:** Python  
- **Main Libraries:**  
  - `scikit-learn` for SVM implementation and model evaluation.  
  - `pandas` and `NumPy` for data manipulation.  
  - `matplotlib` and `seaborn` for visualizations.  
- **Development Environment:** Jupyter Notebook  

## **How to Use the Project**  
1. Clone this repository:  
   ```bash
   git clone https://github.com/SebasKHE/Tumor-Classification-SVM.git
   ```
2. Install the required dependencies:  
   ```bash
   pip install scikit-learn
   pip install pandas
   pip install matplotlib
   pip install seaborn
   ```
3. Open the notebook:  
   ```bash
   jupyter notebook notebooks/svm_tumors.ipynb
   ```
4. Run the cells to train the model and evaluate its performance.

## **Conclusion**  
This project demonstrates the potential of Support Vector Machines in solving binary classification problems in medical contexts, achieving reliable performance that can contribute to early tumor diagnosis.

---
