# Predicting Marketing-Driven Sales and Comparing Channel Performance

## 📋 Project Overview  
This project analyzes the performance of marketing campaigns to determine the most effective strategies for maximizing sales conversions. By leveraging advanced supervised machine learning models, the project aims to:  
- Predict sales conversion rates.  
- Evaluate and compare the effectiveness of different marketing channels.  
- Provide actionable insights to optimize marketing investments and improve ROI.  

---

## 📊 Key Objectives  
1. **Forecast Sales**: Predict sales conversion rates to guide future marketing strategies.  
2. **Compare Marketing Channels**: Assess and rank channels based on ROI and effectiveness.  
3. **Identify Key Drivers**: Determine the most impactful features (e.g., ad spend, audience engagement) for marketing success.  

---

## 📁 Data Source  
- **Original Dataset**: [Marketing Campaign Performance Dataset](https://www.kaggle.com/datasets/manishabhatt22/marketing-campaign-performance-dataset/data)
-  Initially, we worked with a dataset focused on **tech companies** within the **tech industry**. However, after exploratory analysis, we discovered that the data exhibited **low variance**, leading to poor model performance.
- **Samples**: 10,000 rows 
- **Updated Dataset**: To address this issue, we explored a new dataset spanning **multiple industries** to ensure greater variance and generalizability.  
- **Final Dataset**: [Digital Marketing Campaigns for SMEs](https://www.kaggle.com/datasets/farhanmittho/digital-marketing-campaigns-for-smes)  
- **Samples**: 10,000 rows  
- **Features**: 43, including engineered interaction terms  
- **Target Variable**: Conversion Rate  

---

## ⚙️ Methodology  

### 1. Data Cleaning & Preprocessing  
- Handled missing values and dropped irrelevant features.  
- Performed one-hot encoding for categorical variables.  
- Scaled numerical features to ensure fair contribution to the model.  

### 2. Feature Engineering  
- Created interaction terms such as `ad_spend_engagement` and `conversion_ad_spend` to capture cross-feature effects.  

### 3. Exploratory Data Analysis (EDA)  
- Analyzed feature distributions and correlations using heatmaps and visualizations.  
- Evaluated marketing channel performance and ROI trends.  
- Identified the low variance in the original dataset and pivoted to a more diverse dataset that included multiple industries.  

### 4. Modeling  
- **Linear Regression**: Baseline model for trend analysis.  
- **Random Forest**: Ensemble model to capture complex relationships.  
- **XGBoost**: High-performance gradient boosting model with feature importance analysis.  

### 5. Model Evaluation  
- Metrics: R², MSE, RMSE.  
- Used SHAP (SHapley Additive exPlanations) to determine feature importance.  

---

## 🛠️ Technologies Used  
- **Programming Languages**: Python  
- **Libraries**:  
  - Data Manipulation: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - Machine Learning: `scikit-learn`, `XGBoost`, `SHAP`  
- **Platform**: Google Colab  

---

## 🗺️ Milestones  

1. **Data Exploration & Cleaning**  
   - Deliverable: Cleaned and structured dataset.  

2. **Feature Engineering & Preprocessing**  
   - Deliverable: Optimized feature set for modeling.  

3. **Model Development**  
   - Deliverable: Linear Regression, Random Forest, and XGBoost models.  

4. **Evaluation & Validation**  
   - Deliverable: Evaluated models with performance metrics.  

5. **Results & Visualizations**  
   - Deliverable: Feature importance analysis, SHAP visualizations, and actionable insights.  

---

## 🌟 Key Insights  
1. **Top Features Driving Conversions**:  
   - `ad_spend`, `conversion_ad_spend`, and `engagement_metric` emerged as the most impactful.  
   - Interaction features like `ad_spend_engagement` were pivotal.  

2. **Dataset Variance Issue**:  
   - The original dataset for **tech companies** exhibited **low variance**, resulting in underperforming models.  
   - By selecting a new dataset spanning **multiple industries**, model performance improved significantly.  

3. **Model Performance**:  
   - **Random Forest**: R² = **0.999**, MSE = **0.00124**  
   - **XGBoost**: R² = **0.997**, RMSE = **0.056**  

4. **Marketing Channel Recommendations**:  
   - Channels with high audience engagement and optimized ad spend delivered the best ROI.  

---

## 🚀 Future Work  
- Incorporate customer segmentation for personalized marketing strategies.  
- Explore ensemble techniques like Stacking and Bagging for further improvements.  
- Integrate external datasets to enrich insights and boost predictive accuracy.  

---

## 👥 Project Team  
- **Chris Nichols**: Project Manager  
- **Isagani Hernandez**: Data Scientist and Contributor   

---

## 📜 License  
This project is licensed under the **MIT License**.  

---

## 📂 Repository Structure  

```plaintext
├── data/                   # Dataset files  
├── notebooks/              # Jupyter Notebooks for development  
├── models/                 # Trained models  
├── results/                # Visualizations, reports, and performance metrics  
├── src/                    # Python scripts for preprocessing, modeling, and evaluation  
├── README.md               # Project documentation  
└── requirements.txt        # Dependencies and libraries  

