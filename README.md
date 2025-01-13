
# 📈**Airbnb Price Prediction with Machine Learning**

This project showcases my expertise in tackling complex data challenges and applying advanced machine learning techniques to predict Airbnb listing prices. The work involved extensive data preprocessing, feature engineering, and robust validation, resulting in a high-performing and interpretable model.

---

## 👁️👁️**Overview**

The goal of this project was to predict Airbnb listing prices using a dataset that included a mix of numerical, categorical, and textual features. The project involved addressing missing data, cleaning text fields, encoding categorical features, and engineering new features to enhance model interpretability and accuracy.

🎯The original dataset consisted of 48 columns and over 15,000 rows, containing a mix of categorical, numerical, and textual data, presenting significant preprocessing challenges.

![image](https://github.com/user-attachments/assets/ddfe0d4b-114e-4a25-9a22-face52c07823)

"The model achieved exceptional metrics, including an MAE of 0.01 and an R² of 1.00, demonstrating high accuracy and predictive power. To address potential overfitting concerns due to these near-perfect metrics, I introduced noise, performed cross-validations, and tested on unseen data to ensure robustness and confirm generalizability.

---

## ✔️**Key Achievements**

- **Advanced Feature Engineering**:
  - **Amenities**: Categorized into `Basic`, `Standard`, and `High` groups and engineered an `amenity_score` to reflect their impact on price.
  - **Property Type**: Assigned weighted tiers (`High`, `Medium`, `Low`) based on historical price trends, improving interpretability.
  - **Content Scoring**: Extracted key phrases from `Summary` and `Description` to compute a `content_score` quantifying listing quality.
  - **Price per Guest**: Added derived features such as `price_per_guest` and `total_beds` for better price modeling.
- **Data Cleaning & Normalization**:
  - Normalized text fields, removed inconsistencies, and handled multilingual content in fields like `Summary` and `Description`.
  - Ensured numerical features were scaled and standardized to improve model training stability.
- **Comprehensive Validation**:
  - Achieved **MAE** and **RMSE** below 0.01 on the log scale, confirming strong model performance.
  - Tested robustness with noisy data and validated generalization using cross-validation and out-of-sample data.

---

## 🛑**Challenges and Solutions**

### 1. **Preprocessing Categorical and Textual Features**
- **Problem**: Inconsistent, sparse, and multilingual data in text fields like `Summary`, `Description`, and categorical features like `Amenities`.
- **Solution**:
  - Cleaned text data to remove special characters, accents, and redundant spaces while preserving context.
  - Assigned weights to `Amenities` and `Property Type` categories based on domain knowledge and price impact.
  - Created a `content_score` from key phrases extracted from text fields, adding predictive value to the model.
- **Outcome**: Enhanced categorical and textual data quality, enabling seamless integration into machine learning workflows.

### 2. **Handling Missing Data**
- **Problem**: Missing values in numerical columns and sparse data in text fields.
- **Solution**:
  - Applied contextual and statistical imputation methods, ensuring alignment with domain logic.
  - Addressed sparse text data by imputing meaningful, context-aligned values.
- **Outcome**: Produced a fully imputed dataset with no missing values, ready for robust training.

### 3. **Feature Selection and Encoding**
- **Problem**: Correlated and redundant features impacted model performance.
- **Solution**:
  - Dropped features like `country_code` due to redundancy with `country`.
  - Selected `neighbourhood_cleansed` over `neighbourhood` based on correlation analysis with price.
  - Used one-hot encoding for categorical data and custom scoring for specific columns (e.g., `Amenities`, `Property Type`).
- **Outcome**: Streamlined features for interpretability while preserving predictive power.

---

## 💡**Results**

- **Performance Metrics**:
  - Achieved **MAE** and **RMSE** below 0.01 on the log scale, confirming exceptional predictive accuracy.
  - Achieved high **R² scores** of ~1.0 across validation and testing, reflecting model reliability.
- **Robustness**:
  - Maintained performance under controlled noise introduction, demonstrating strong generalization capability.
- **Feature Importance**:
  - SHAP analysis highlighted key contributors like `amenity_score`, `price_per_guest`, and `accommodates`.

---

## **Visualizations**

- **Residual Analysis**: Showed minimal bias and well-distributed errors, confirming good model fit.
- **Predictions vs. Reality**: Scatter plots revealed tight alignment between predicted and actual values.
- **Loss Curves**: Visualized training and validation losses using Huber Loss and L2 Regularization, showcasing convergence and stability.

---

## 💻**Technical Stack**

- **Programming**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, TensorFlow/Keras, SHAP, Matplotlib
- **Techniques**:
  - Feature engineering (e.g., scoring, derived features, text processing)
  - Advanced imputation strategies for text and numerical data
  - Robust model training with Huber Loss and L2 Regularization

---

## 🤓**Workflow Key**

- **Preprocessing Excellence**: Solved real-world data challenges, including multilingual content, missing data, and redundant features.
- **Feature Engineering Expertise**: Created meaningful derived features, improving both interpretability and performance.
- **Scalability**: Designed workflows to handle messy, real-world datasets, ensuring model robustness across noise and variability.

---
