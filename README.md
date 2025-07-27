# LDA_Heart_Failure_Classification

This project applies **Linear Discriminant Analysis (LDA)** to classify heart failure patients based on smoking status using selected clinical indicators. The dataset includes medical records from patients with heart conditions, and the goal is to explore whether LDA can effectively discriminate between smokers and non-smokers.

---

## 📊 Dataset

- **Source**: [Heart Failure Clinical Records Dataset](https://www.kaggle.com/datasets/andrewmvd/heart-failure-clinical-data)
- **Format**: `.xlsx`
- **Target Variable**: `smoking` (converted to factor with levels "A" and "B")
- **Features used**:  
  - `age`, `serum_sodium`, `platelets`, `serum_creatinine` (selected via stepwise method)

---

## 🔍 Project Steps

1. **Exploratory Data Analysis**
   - Spearman correlation matrix
   - Summary statistics and normality tests (Shapiro-Wilk)

2. **Assumption Checking**
   - Univariate & multivariate normality
   - Homogeneity of covariance matrices (Box’s M test)

3. **Linear Discriminant Analysis**
   - Model fitting with selected features
   - Coefficients and discriminant function
   - Group prediction and comparison

4. **Model Evaluation**
   - Classification accuracy
   - Prior probability baseline
   - Visualization (histogram of LDA scores)

5. **Feature Selection**
   - Stepwise selection using `greedy.wilks()` (klaR package)

---

## 📦 R Packages Used

- `readxl`
- `corrplot`
- `funModeling`
- `rstatix`
- `biotools`
- `MASS`
- `klaR`
- `dplyr`

---

## 📈 Output

- LDA classification accuracy
- Visualized separation between classes
- Comparison between predicted and actual labels

---

## 🧠 Key Insight

> LDA can be a powerful classification tool even with few predictors, provided assumptions like normality and homogeneity are reasonably met. In this dataset, classification based on lab values and patient features yields insightful group separation.

---

## 💬 Contact

For questions or feedback: [Melda Korkudan](https://github.com/melldaa)

