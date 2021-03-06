## Machine learning framework for prediction of patient-hospital readmission in US.

The dataset is available in the UCI repository as [Diabetes 130-US hospitals for years 1999-2008 Data Set](https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008#). 

- The data was collected from 130 hospitals in the U.S. during 10 years(1999-2008)
- Contains 101,766 observations and 50 features, including demographic attributes, diagnostics, medications and hospital outcome.

This project is divided in two parts associated with the data preparation and the classification models. 
- *Data Preparation*:
Since the original database contains incomplete, redundant, and noisy information it was necessary implement a data wrangling process to remove duplicates, check missing values, recategorize some variables and remove other ones. The final dataset contains 56.195 records and 56 attributes, having the readmission status in the first 30 days as the binary outcome. This dataset consists of hospital admissions that did not result in a patient death or discharge to a hospice. Each encounter corresponds to a unique patient diagnosed with diabetes, although the primary diagnosis may be different.

- *Classification models*:
The best two models found are: Random Forest and Logistic Regression through an oversampling approach to balance the dataset.

### Conclusions

* Using oversampling to balance the classes guarantee a better performance since most of the machine learning algorithms needs a similar proportion into the classes.
* After checking with various machine learning models, for classify the patients minimizing the error of readmission, my suggestion is to use the *Random forest* model since it has the best performance.
* For identifying risk and protective factors my suggestion is the *Logistic Regression* model since it is the second best model and it is interpretable.
    * The top three of protective factors are: not being in Emergency as admission type, have any change in the diabetics medications and  have any diabetic medication.
    * When the patient has been more in contact with the hospital: more days in the hospital, more procedures or more outpatient visits, the odds of being readmitted decrease.
    * The top three of risk factors are: number of inpatient visits, the discharge is not at home,  number of diagnoses reported into the system.
