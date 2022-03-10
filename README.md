# Loan Dataset Exploration (Dataset Exploration Title)
## by Davit Lomadze


## Dataset

Dataset provides information about loan. Dataset contains detailed information about loans and borrowers. Dataset contains both qualitative and quantitative measurements.Data contains 81 measurements and 113,937 observations. First of all unecessary columns were dropped. Then any missing data that couldn't be replaced also got dropped. A new column was added, which has mid point of lower and upper ranges of credit score as values.



## Summary of Findings

In our exploration was discovered that `Term`, `CreditScore` and `DebttoIncomeRatio` seem to have very low correlation with `BorrowerAPR`. The calculation of APR consists of loan [term](https://www.investopedia.com/terms/a/apr.asp), thus term not having effect on APR doesn't seem logical. There could be other influencing factors, that could have affect together with DebtToIncomeRatio and Term.

Regardless, the direction of the correlation is logical. Term to BorrowerAPR correlation is negative, meaning the less the Term is, the higher APR gets, which makes sense if we judge by the equation. In case of DebtToIncomeRatio, correlation is positive, because high ratio means increased risk of not being able to pay the loan, thus higher APR. In case of CreditScore, also lower the credit score the higher is the risk, thus higher APR.

If we compare medians by `Occupation`, we can notice Engineers and Computer Programmers have lowest APR median. We can observe that Executives, Engineers, Analysts and Computer Programmers have lowest median of APR. By EmploymentStatus Full-time employees have lowest median. By IncomeRange borrowers with 100,000+ income have lowest median APR and with 1-24,999 highest, which makes sense. Suprising is the fact, that 0 and not displayed income APRs aren't higher compared to others. By Employment status self-employed have lowest median APR. Mostly, given results follow basic logic of lesser the risk the lesser tha APR.

We observed that higher credit score means lower apr, which is not suprising. Also, very interesting trend, occupations with lower APR also have lower Debt-to-Income ratio, meaning they carry less risk for lender and provide lesser APR.

Analysing income range by state reveales that regardless of which income range is prevelant, isn't showing connection with APR. Thus, in further analysis combining state and income range wouldn't make picture clearer, because it seems APR is affected by inner state monetary policies. It clear that within states with stricter monetary policy there will be higher interest rates, but we mostly interested how our actions can affect the apr. Because of this, states will be omitted from further analysis.

Multivariant observation showed strong relationship between occupation, income range, debt to income ratio and creditscore. The connection with creditscore was obvious, it is influenced by income and debt to income ratio. In all observations the pattern over all is similar, high income and creditscore, low debt to income ratio means lower apr.

When we observe interaction between income range and apr by occupations, in some cases apr is lower on low income range rather than high income range. Such occupations are accountant, engineer, analyst and computer programer. This is out of ordinary and would require farther investigation.

Observations revealed, main determinanat of apr is income range, debt to income ratio and credit score. Occupations that have lowest median apr are engineers, executives, computer programers and analysts, because they have highest income range and lowest debt to income ratio with high credit score. But it doesn't mean that only profession will decide apr. Maintaining low debt to income ratio and high credit score will have influence on apr, might not become as low as for above mentioned professions, but can be observed it can be lowered.

## Key Insights for Presentation

First Borrower APR will be introduced, how it is distributed. We will observe how income, debt to income ratio, credit score and lastly how APR is distributed by occupation of the borrowers. If occupation reflects income and debt to income ratio, we should see that same occupations have advantages situation in terms of nagotiating for lower APR. Meaning if certain occupations have high income range and low debt to income ratio, they should get lower apr.
