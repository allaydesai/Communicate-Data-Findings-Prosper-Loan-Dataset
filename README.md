# Communicate-Data-Findings-Prosper-Loan-Dataset
Perform univariate, bivariate and multivariate analysis on factors affecting borrower’s APR interest rate

**UDACITY** | Data Analyst Nanodegree Program

---

### OVERVIEW

Data visualization is an important skill that is used in many parts of the data analysis process. Exploratory data visualization generally occurs during and after the data wrangling process, where we understand the patterns and relationships present in your data. Explanatory data visualization techniques are used after generating your findings, and are used to help communicate your results to others.

The goal of this project is to demonstrate the importance and value of data visualization techniques in the data analysis process. In the first part, Python visualization libraries are used to systematically explore Prosper Loan dataset, starting from plots of single variables (Univariate) and building up to plots of multiple variables (bivariate and multivariate). In the second part, a short presentation was created which illustrates interesting properties, trends, and relationships that were discovered in the dataset. The exploratory visualizations from the first part were transformed into polished, explanatory visualizations.

### DEPENDENCIES

The following libraries are required to run this project:

- Python
- NumPy
- pandas
- Matplotlib
- Seaborn

### PROJECT FILES
<ul>
  <li>Prosper_Dataset_Exploration.ipynb</li>
  <li>Prosper_Dataset_Exploration.html</li>
  <li>prosperLoanData.csv</li>
  <li>SlideDeck.ipynb</li>
  <li>SlideDeck.html</li>
  <li>README.MD</li>
</ul>

### DATASET

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

For the purpose of this analysis following variables were chosen:

**Numerical** 

| Column Name |
|----------|
| BorrowerAPR |
| LoanOriginalAmount |
| ProsperScore |
| StatedMonthlyIncome |
| Occupation |
| CreditScoreRangeLower |
| CreditScoreRangeUpper |
| AvailableBankcardCredit |
| RevolvingCreditBalance |

**Categorical**

| Column Name |
|----------|
| Term |
| ProspectRating (Alpha) |
| EmploymentStatus |

### SUMMARY OF FINDINGS

Upon completion of data exploration it was found that Borrower APR had a multimodal shape data distribution with few peaks. Borrower's APR negatively correlated with loan origination amount, i.e. with increase in loan amount there was a drop in borrower APR. Further Prosper score and prosper rating seem to have the strongest effect on borrower APR. It was found that borrowers with higher Prosper ratings had lower Borrower APR. When we compared borrower APR with loan amount for each prosper rating, an interesting trend was observed. For most lower ratings, a negative relationship was observed as expected but for some higher ratings we did see a slightly positive relationship such that for larger loan amounts under those prosper ratings, borrower APR increased. It was also observed here that rating B & C had larger number of loans. Another interesting finding was observed when looking at the distribution of state monthly income which was skewed to the left, majority of the borrowers had an income less than $40k. Next, when effects of occupation on APR was explored, we found that borrower's APR was same between the various occupations, this seemed unexpected as I would have expected there to be a trend. Credit score showed a similar trend as prosper score where better credit score resulted in lower borrower APR which was to be expected and most borrowers were within 650 to 780 range.

When looking at categorical variables, it was found that term size has a direct impact on loan origination amount. This is to be expected as most people want to keep their monthly liability relatively low hence with increase in loan amount the term length would have to increase. Loan amount increases as the term for loan increases. There is a positive relationship between Borrower APR and Prosper Rating. It was observed that the APR is low with better rating. Lower APR was seen by employment status: Employed, Full-time and Self-Employed.

### KEY INSIGHTS FOR PRESENTATION

For the presentation, the goal was to showcase all the features that have a significant impact on Borrower APR. Once again here you can see that Prosper Score has strongest relationship with Borrower APR. I begin with showing a distribution of Borrower APR and Loan origination amount followed by a comparison of Borrower APR against Prosper Score and Loan Origination amount against Term. Finally, effects of prosper rating on the relationship between Borrower's APR and Loan Origination Amount was explained which was followed up by reaffirming the strong relationship between Borrower APR and Prosper Score.
