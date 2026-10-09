# Bank Marketing Campaign Analysis

## Project Overview

This project analyzes bank marketing campaign data to identify customer characteristics and campaign-related factors associated with term deposit subscriptions. The goal is to generate insights that can help a bank plan more targeted and effective marketing campaigns.

## Business Problem

Banks spend time and resources contacting customers to promote financial products. Understanding customer response patterns can help the bank evaluate campaign performance, identify relevant customer segments, and improve future campaign planning.

## Project Objectives

* Understand and validate the dataset.
* Clean and prepare data for analysis.
* Perform Exploratory Data Analysis (EDA).
* Analyze customer characteristics and campaign interactions.
* Apply statistical tests to examine relationships with deposit subscription.
* Create meaningful customer segments through feature engineering.
* Develop actionable business insights and recommendations.

## Dataset Overview

* **Records:** 11,162
* **Columns:** 17
* **Target variable:** `deposit`
* **Target values:** `yes` and `no`

The dataset includes customer demographics, financial information, current campaign interactions, previous campaign history, and subscription outcomes.

### Main Variables

* **Customer characteristics:** `age`, `job`, `marital`, `education`, `default`, `balance`, `housing`, `loan`
* **Current campaign:** `contact`, `day`, `month`, `duration`, `campaign`
* **Previous campaign:** `pdays`, `previous`, `poutcome`
* **Target:** `deposit`

## Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn, if used in the notebook
* SciPy for statistical testing

## Data Cleaning and Validation

* Converted invalid numeric entries into missing values.
* Checked missing values and duplicate records.
* Validated numerical ranges and categorical values.
* Investigated potential outliers using the Interquartile Range (IQR) method.
* Identified implausible ages and handled them using median imputation.
* Retained extreme values when they could represent legitimate customer or campaign observations.

## Exploratory Data Analysis

The analysis examined:

* Deposit subscription distribution.
* Customer age and job categories.
* Education, housing loan, and personal loan status.
* Contact methods and campaign activity.
* Previous campaign outcomes.
* Relationships between customer segments and deposit subscription.

## Statistical Analysis

* **Chi-square test:** Examined associations between categorical variables and deposit subscription.
* **Welch's t-test:** Compared numerical variable means between customers who subscribed and those who did not.

Statistical significance indicates evidence of an association or difference; it does not establish causation.

## Feature Engineering

Created grouped variables to simplify business interpretation:

* Age groups.
* Current campaign contact-frequency groups.
* Previous-contact groups.

## Key Findings

* Customers with a successful previous campaign outcome had a particularly high observed subscription rate.
* Subscription rates varied across job and age groups.
* Customers contacted more frequently during the current campaign showed lower observed subscription rates in the analyzed data.
* Subscription rates differed by education, housing loan status, personal loan status, and contact method.
* Previous campaign history provided useful information for customer segmentation.

## Business Recommendations

* Use customer characteristics and campaign history to develop meaningful customer segments.
* Consider previous campaign outcomes when prioritizing future marketing activities.
* Review repeated-contact strategies to investigate potential diminishing returns.
* Compare communication channels using response rates, costs, and customer experience.
* Evaluate both segment size and subscription rate before prioritizing a customer group.
* Validate findings with future campaigns before making major operational changes.

## Limitations

* The analysis is based on historical observational data.
* Associations do not prove cause-and-effect relationships.
* Call duration is known during or after a call, so it should be treated carefully for pre-call targeting.
* Extreme values may be legitimate and should not be removed without business justification.
* Future campaign data can help validate whether these patterns continue.

## How to Use This Project

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook.
4. Ensure the CSV dataset is available at the file path used in the notebook.
5. Run the notebook cells to reproduce the analysis.

## Conclusion

This project uses Python-based data analysis and statistical testing to identify customer and campaign patterns associated with term deposit subscription. The findings provide a foundation for customer segmentation and more informed marketing campaign planning.
