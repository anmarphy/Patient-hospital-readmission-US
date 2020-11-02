# Globant Data Scientist Assesment

## Machine learning framework for prediction of patient-hospital readmission in US.

The dataset is available in the UCI repository as [Diabetes 130-US hospitals for years 1999-2008 Data Set](https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008#). 

- The data was collected from 130 hospitals in the U.S. during 10 years(1999-2008)
- Contains 101,766 observations and 50 features, including demographic attributes, diagnostics, medications and hospital outcome.

This project is divided two parts associated with the data preparation and the binary classification.To have a better visualization of the scripts, I suggest to check them in nbviewer:
- *Data Preparation*:
The final dataset contains 56.195 records and 56 attributes, having the readmission status as the outcome. This dataset consists of hospital admissions that did not result in a patient death or discharge to a hospice. Each encounter corresponds to a unique patient diagnosed with diabetes, although the primary diagnosis may be different.

- *Classification models*:
The best two models found are: Random Forest and Logistic Regression through a oversampling approach to balance the dataset.

### Conclusions
-  After checking with various machine learning models, for classify the patients minimizing the error of readmission, my suggestion is to use the Random forest model since it has the best performance. And for identifying risk and protective risk my suggestion is the logistic model since it is the second best model and it is interpretable.
- The top three of protective factors are: not being in Emergency as admission type, have any change in the diabetics medications and  have any diabetic medication.
- When the patient has been more in contact with the hospital: more days in the hospital, more procedures or more outpatient visits, the odds of being readmitted decrease.
- The top three of risk factors are: number of inpatient visits, the discharge is not at home,  number of diagnoses reported into the system.
