# KrishiSahayak

### Predicting Distress Risk Before Harvest Using Rainfall, Temperature, and Historical Yield Patterns Across Maharashtra Districts

## About the Research

KrishiSahayak is a machine-learning research project focused on classifying agricultural distress risk across Maharashtra districts before the end of a growing season.

The study examines the relationship between rainfall variation, temperature, sown area, and historical crop-yield patterns to classify district–crop combinations into three risk categories: Low, Medium, and High.

The objective is to explore how predictive modelling can support earlier identification of agricultural risk and help inform agricultural planning and support interventions.

## Research Objectives

* Prepare a model-ready dataset combining agricultural statistics with rainfall and temperature records.
* Engineer historical features while avoiding the use of current-season yield as a model predictor.
* Compare Logistic Regression with XGBoost.
* Evaluate the models using test-set metrics and stratified cross-validation.
* Examine feature importance to understand which variables contribute most to predictions.
* Explore the use of a bilingual English–Marathi Streamlit dashboard for presenting risk assessments.

## Methodology

The research uses district-level, crop-wise, and year-wise observations.

**Key input features:**

* Rainfall and rainfall deviation
* Average temperature
* Area sown
* Previous-year crop yield
* Three-year average yield
* Historical yield variability

**Models evaluated:**

* Logistic Regression — baseline model
* XGBoost — main model

**Evaluation methods:**

* Stratified train-test split
* Five-fold stratified cross-validation
* Accuracy, precision, recall, macro-F1, and ROC-AUC

## Key Findings

In the reported test-set results, XGBoost achieved:

* **Accuracy:** 63.9%
* **Macro-F1:** 0.638
* **ROC-AUC:** 0.816

Logistic Regression achieved 57.5% accuracy and a macro-F1 score of 0.570 on the same test evaluation.

Rainfall deviation from a district's historical average was identified as the strongest feature in the reported analysis.

These results describe the performance on the dataset used in this study and should not be interpreted as proof of performance on future seasons without further testing.

## Limitations

* Rainfall and temperature records were unavailable for 2010 and 2011 in the source dataset.
* The analysis does not include district-level market prices or financial-loss data.
* The model uses tabular data rather than satellite imagery.
* The Medium-risk category was more difficult to classify than the High- and Low-risk categories.
* The study's historical data ends in 2017, limiting conclusions about present-day agricultural conditions.

## Research Paper

The complete research paper is available in this folder:

**`KrishiSahayak-Research-Paper.pdf`**

## Technologies and Methods

Python · Pandas · Scikit-learn · XGBoost · Streamlit · Predictive Modelling · Exploratory Data Analysis

## Author

**Durva Ambre**
TY BSc Data Science and Analytics

---

*An academic research project exploring machine learning for agricultural risk assessment.*
