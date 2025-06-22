# Data-Driven-Loan-Risk-Assessment-using-Advanced-Excel
This project uncovers patterns that predict installment repayment difficulties, enabling the lender to deny loans, reduce amounts, or charge higher interest to risky applicants. By identifying the key drivers of default, the company can refine approval criteria, minimize losses, and avoid rejecting credit-worthy borrowers.


Main problems to be solved

* incomplete applicant profiles
  many urban borrowers lacked credit history or had gaps in their data, making their repayment ability hard to judge
* dual risk of misclassification
  • approving a high-risk borrower leads to losses
  • rejecting a credit-worthy borrower means lost revenue
* hidden patterns in defaults
  without systematic analysis, the drivers behind first-installment payment delays remained unclear

How I solved it

* Mapping & Imputing Missing Data
  • addressing incomplete applicant profiles by filling blanks with median values, I ensured every case could be evaluated rather than automatically rejected for “unknown” credit factors
* Identified and reviewed outliers
  • computed Q1, Q3 and IQR with QUARTILE functions
  • used conditional formatting to highlight extreme entries
  • addressing hidden risk factors among approved borrowers by flagging extreme income or repayment-behavior values I helped spot applicants who looked good on paper but fell outside normal patterns.
* measured class imbalance
  • leveraged COUNTIF and SUM to get counts of late-payers vs on-time payers
  • visualized each distribution with pie charts and stacked‐bar charts to spotlight skew.
* conducted univariate, segmented univariate and bivariate analysis
  • generated column chart for each variable thus identifying which category had more difficulty in paying loans compared to the other
  • with the help of bivariate analysis involving different factors against default rates, I identified high-risk segments which helped streamline approval criteria to reduce bad loans without turning away good borrowers.
* drilled down with pivot tables
  • cross-tabulated borrower attributes against application outcomes
  • spotted segment-specific trends in loan approvals and defaults
* surfaced top predictors via correlation
  • calculated CORREL between each attribute and default status within segments
  • plotted heatmaps to highlight the strongest indicators of repayment trouble
