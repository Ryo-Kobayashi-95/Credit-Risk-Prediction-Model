# Report: Credit Default Risk Assessment Model

Published: Jun 3, 2023

Author: Ryo Kobayashi

* For the complete report, please refer to the provided "Report.ipynb" above.

<br/>

## *Abstract:*
In the dynamic and ever-evolving landscape of finance, precision in risk assessment stands as a cornerstone for credit institutions. Within this context, the present project embarks on a compelling journey—the construction of a predictive machine-learning model poised to address the pivotal challenge of client default risk. By harnessing the power of predictive analytics to anticipate credit card payment defaults, this model wields the potential to infuse vital intelligence into lending decisions, resource allocation, and the formulation of effective risk management strategies.

At the heart of this endeavor lies a comprehensive dataset meticulously curated from Taiwan, serving as the bedrock upon which the model's architecture is built. This dataset encapsulates a wealth of information, ranging from multifaceted demographic insights to intricate payment histories and credit data. The fusion of these diverse attributes creates a robust foundation for the model's predictive capabilities.

This report serves as an exploration into the intricate mechanics that underpin this predictive model. It traverses through the model's inner workings, spotlighting its remarkable ability to assimilate and synthesize historical trends and multifarious attributes. This synthesis, in turn, significantly enhances the model's efficacy in risk assessment and its potential to unravel the complex tapestry of credit behavior patterns.

As the report delves deeper, it peels back the layers of complexity that often shroud credit default risk. Through an exploration of the model's functionality, readers are invited to witness firsthand how the integration of diverse data facets contributes to a more holistic and accurate prediction of default risk. By doing so, this report not only showcases the capabilities of machine learning in finance but also sheds light on the intricate interplay between data, analytics, and prudent financial decision-making.

## *Target Audience:*
This project is tailored to individuals curious about the interplay between machine learning and finance. Whether you're an aspiring data scientist, an innovative financial analyst, or a researcher at the crossroads of technology and finance, this project provides valuable insights. *It's important to note that while the project provides valuable insights, its practical application is not advisable due to its experimental nature*.

## *Project Motivation:*
Driven by my academic journey and passion for finance, I'm motivated to uncover the latent power of risk assessment in shaping informed financial decisions. This project acts as a guiding light, showcasing how machine learning can transform risk management. Going beyond theoretical knowledge, it offers a holistic grasp of real-world applications, bridging the gap between theory and practice, and enabling the utilization of data-driven insights in the complex realm of finance.

## *Stages in Model Creation:*

### 1. Preliminary Exploratory Data Analysis (EDA):
- The initial stage involved reading and partitioning the data into a training set (70%) and a testing set (30%).
- Summary statistics were computed to assess data consistency and identify potential class imbalance.
- Visual analysis was conducted using histograms and bar plots to uncover correlations among features.
- A suitable evaluation metric, determined to be the f1 score, was chosen.

#### Histogram
![image](https://github.com/Ryo-Kobayashi-95/Credit-Risk-Prediction-Model/assets/115038173/b30f2586-3b8c-4508-be59-3eb67125dd62)

#### Barplot
![image](https://github.com/Ryo-Kobayashi-95/Credit-Risk-Prediction-Model/assets/115038173/1eb3a147-92a5-4472-8899-7c48dad01617)

### 2. Preprocessing and Transformation:
- Numeric columns were standardized using the StandardScaler.
- Categorical columns were transformed using OneHotEncoder (OHE).

### 3. Model Construction and Hyperparameter Tuning:
- Various machine learning models were constructed, including Baseline, LogisticRegression, DecisionTreeClassifier, KNeighborsClassifier, RandomForestClassifier, and SVC.
- Hyperparameters were optimized for each model.
- Model selection was based on the test f1 score and fitting time, with LogisticRegression being chosen as the best model.

#### Best model performance
![image](https://github.com/Ryo-Kobayashi-95/Credit-Risk-Prediction-Model/assets/115038173/2fa081a4-38a5-4f61-9818-f2a14ce2cc0a)

### 4. Model Deployment and Results:
- The selected LogisticRegression model was deployed on the test data.
- The model achieved an f1 accuracy of 0.46.

### 5. SHAP Analysis:
- SHAP analysis was conducted to interpret the model's predictions. However, there is no detailed description of the SHAP analysis process in the provided text.

#### SHAP Force Plot
![image](https://github.com/Ryo-Kobayashi-95/Credit-Risk-Prediction-Model/assets/115038173/41c52930-d79e-43b5-9706-e6d79e8035c4)

<br/> <br/> 

## *Source*
Dataset retrieved from: https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset
