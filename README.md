# Factors that affect the outcome of a loan

## by Charles Nikoro

## Dataset

The dataset used for this investigation is the Prosper loan dataset retrieved from Udacity. It comprises 113937 observations and 81 variables which comprises both qualitative and quantitative variables.

I only considered loans that were either completed, defaulted, or charged-off. Apart from the main variable of interest, `LoanStatus`, others explored in this investigation are: `LoanOriginalAmount`, `LP_CustomerPrincipalPayments`,`BorrowerAPR`, `LP_InterestandFees`, `Term`, `LoanCurrentDaysDelinquent`, `EmploymentStatus`, `ListingCategory (numeric)`, and `TotalProsperLoans`.

`EmploymentStatus` variable comprises of "Not employed", "Full-time", "Part-time", "Retired", "Employed", "Self-employed", "Other", and "Not available" categories. For this investigation, I only considered records whose employment status are known. Therefore, records with an "Other" or "Not available" status where not considered. Also, since it is safe to assume that borrowers with a "Full-time" and "Part-time" status have an employer, I merged them with those whose status is "Employed". Consequently, the categories of employment status considered are "Not employed", "Self-employed", "Employed", and "Retired".

## Summary of Findings

From my investigation, I found that employment status, annual percentage rate, term of the loan, principal outstandings (which is the difference between the loan original amount and the amount of principal paid), and the number of days a borrower is delinquent are possible factors that can affect the loan outcome.

An interesting observation is that borrowers that are unemployed and have the "Defaulted" or "Chargedoff" status are been delinquent for a considerable amount of days that is lesser than those of other employment status. This might be because they are assumed to be unable to complete their payments ones they are past due for some days.

An increase in the annual percentage rate was observed as I analyzed completed, defaulted, and charged-off records. The principal outstanding was also observed to increase as the loan term increases. This trend was observed with defaulted and charged off records. Records of completed loans do not have principal outstandings as expected.

As expected, I observed an increase in the number of days of delinquency as I analyzed completed, defaulted, and charged-off records.

## Key Insights for Presentation

For the presentation, I focus on the influence of the principal outstanding, the number of days borrowers were delinquent, the loan term, and the employment status on the outcome of the loan. I start by introducing the `LoanStatus` variable followed by each of the distributions of `LoanPrincipalOutstanding` and `LoanCurrentDaysDelinquent`. This is followed by box plots of each of these variables and the `LoanStatus`.

Afterwards, I introduce each of the categorical variables. To start I use the box plot of the loan status and principal outstanding across the loan term. Next, I use the box plot of the loan status and number of days borrowers were delinquent across the loan term. Finally, I use the box plot of the loan status and the number of days borrowers were delinquent across the employment status, and did the same with the box plot of the loan status and the principal outstanding.
