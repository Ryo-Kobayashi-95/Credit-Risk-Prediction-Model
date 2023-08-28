# Report: Credit Default Risk Assessment Model

Published: Jun 3, 2023

Author: Ryo Kobayashi

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
1. **Data Splitting:** The dataset was divided into a 70% training set and a 30% testing set.
2. **Preliminary Exploratory Data Analysis (EDA):** The data structure was uncovered, necessitating preprocessing before constructing machine-learning models.
3. **Metric Choice:** The test f1 score, derived from EDA, was selected as the most suitable evaluation metric for the project.
4. **Model Building:** Various linear and non-linear models (e.g., LogisticRegression, DecisionTreeClassifier, KNeighborsClassifier, and SVC) were constructed, and hyperparameters were tuned to maximize the test f1 score.
5. **Model Selection:** Considering the test f1 score and fitting time, LogisticRegression was identified as the optimal model, subsequently deployed on the test set.
6. **SHAP Analysis:** SHAP force plots were utilized to unveil influential factors driving model outcomes.
