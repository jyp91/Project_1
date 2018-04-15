# Project 1 Standardize Test

**Introduction:**
The primary focus of this project is to understand the basic concept of data analysis process by using datasets that cotains the SAT and ACT test scores of graduating class in 2017 from PrepScholar. This project highlights the basic process of data cleaning, exploratory data analysis (EDA), creating visualizations (histograms and scatter plots), conducting A/B testing and generating 95% confidence intervals.

**Data Cleaning:**
By checking the overall datasets information and type, column unnamed: 0 were dropped for both datasets since it represents index column. In addition,  participation column for both datasets was converted into float since it represents the numerical value of student participation rate for the ACT and SAT test.  Moreover, ACT and SAT datasets were merged into one dataset on State column. Lastly, the new data frame was created by renaming and rearranging the columns separated by the ACT and SAT columns with the combined dataset.

**Exploratory Data Analysis:**
The participation rate for ACT shows negative skew whereas SAT shows positive skew distribution, explaining more students are participating ACT test over SAT. In addition, students tend to score higher on SAT math compared to ACT math by showing the positive skew histogram for SAT and evenly distributed scores that range from 18 to 25 for ACT.  However, scores for English or Evidence-Based Reading and Writing for both tests show a similar trend by forming a bell curve shape histogram that ranges from low to high. Overall, students score higher on SAT than ACT. The box plot shows that the mean of ACT composite score is approximately 40% away from the max score 36 and mean of SAT total score is approximately away from the max score 1600 by 36%.

**A/B Test:**
The hypothesis test that compares the SAT and ACT participation rates as follows.

**H0: μSATParticipation = μACTParticipation**

**HA: μSATParticipation ≠ μACTParticipation**

Based on the A/B test result by using scipy stats model, pvalue was equal to 0.000241342036.  This result can be concluded by rejecting the null hypothesis since the pvalue is less than alpha (α=0.05).
Also,  with 95% confidence intervals for SAT and ACT participation rates are in between -31.05 and 110.66 for SAT and  0.69 to 129.81 for ACT.

**Conclusion:**
The results of A/B testing and 95% confidence intervals were different despite the fact that both tests cover the same domain field. Also, the trend in standardized test taking is shifting towards ACT test. This result could be due to the difference in price and the test difficulty. The additional data source could answer these questions.
