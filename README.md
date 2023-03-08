# credit-risk-classification
## **Module 20 Challenge -- Credit Risk Classification for UCI Data Analytics Bootcamp**

## Vincent Passanisi

## Due March 13, 2023

---

# **Introduction**

The purpose of this challenge was to build a prediction model that would be able to analyze credit worthiness of borrowers for a bank and flag potential loan defaults. The dataset provided by the bank contained 77,536 entries with seven key indicators. These are listed as follows:

* Size of the loan
* Interest rate on the loan
* Borrower's income 
* Debt_to_Income ratio
* The number of of accounts that the borrower uses regularly
* Derogatory marks on the borrower's credit report
* The borrower's total debt

A final column called *loan status* was provided that indicated a healthy loan with a `0` and a loan in default with a `1`.

<br/><br/>

# **Files**

In the repository are the completed challenge files.

* *README.md* - ReadMe file for the project.
* *Credit_Risk* folder contains the resources folder and challenge files
    * *credit_risk_classification_complete.ipynb* - **completed Jupyter notebook**.
    * *credit_risk_classificationr* - provided Jupyter notebook with starter code.
    * *report-complete.md* - completed analysis report
    * *report-template.md* - provided template for the anylsis report.
    * *Resources* folder - contain the *lending_data.csv* with loan data
<br/><br/>

# **Results**

Detailed results are provided in the analysis report which can be found in the *Credit_Risk* folder in this repository.
A link to the document can be found here: [Completed Analysis Report](https://github.com/vgpass/credit-risk-classification/blob/main/Credit_Risk/report-complete.md)

# **Comments and Thoughts**

I found this assignment to be straight-forward and much easier for me than previous challenges. Most of my time was spent on the report and README, and getting all the details right. I am feeling more and more confident with my python and pandas abilities with every assignment. I played around with the data a little just to add some details of interest. Simple things, but I think they added to the overall report. For instance, I got the total loans outstanding from the dataset, and figured out the percentage of those loans that were in default. I thought this information was crucial in convincing the bank of the importance of getting an accurate model. When you have 46 million dollars in loans that could go into default, you definitely want to put some resources into it.

Some administrative details I would like to address have to do with the instructions for the assignhment. First, the assignment was never uploaded to GitLab. Not sure why that was. Also, the report template seemed to be asking for us to use two different prediction models and compare them, but the starter code asked us to use only one model, Logistic Regression, and then refit the model using random data generated using an oversampling module. This didn't faze me at all, I just did a little research and figured it out. Although it wasn't something discussed in class, the documentation was straightforward and after a bit of reading, I was back on track. Finally, the instructions on canvas referred to a subsection called **Predict a Logistic Regression Model with Resampled Training Data**, but there is no such section in the instructions. Something that may need to be fixed for future cohorts. :-)

Enjoyed this one a lot, and learned quite a bit.







