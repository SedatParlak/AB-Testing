### What is A/B testing ?

The two-sample t-test (also known as the independent samples t-test) is a method used to test whether the unknown population means of two groups are equal or not. A two-sample t-test is used to analyze the results from A/B tests. You can use the test when your data values are independent, are randomly sampled from two normal populations and the two independent groups have equal variances.

AB Testing Steps:

* 1- Create a hypothesis
* 2- Assumptions check
  * Assumption 1: Distributions are normal for each variable
  * Assumption 2: Variances are homogeneus
* 3- Apply the hypothesis and control p value. If p value is less than 0.05 we can reject the HO if not we can accept HO. 
 * a) If the assumptions are correct use the independent samples t-test (parametric test, t test)
 * b) If the assumptions are not correct use the mannehitneyu test (non-parametric test, mannwhitneyu)
 
**Note**: If assumption 1 is not correct we can use directly non-parametric test (option b). If assumption 1 is correct but assumption 2 is not, we can use the parametric test and add that variances are not homogeneus as a argument.


### About this work
#### A/B Testing - Comparing Bidding Methods
Problem: Facebook recently introduced a new bidding type, "average bidding", as an alternative to the existing "maximum bidding" bidding type. One of our customers, bombabomba.com, decided to test this new feature and would like to do an A/B test to see if average bidding converts more than maximum bidding. A/B testing has been going on for 1 month and now bombabomba.com is waiting for you to analyze the results of this A/B test from us. Purchase is the ultimate success criterion for Bombabomba.com. Therefore, the Purchase metric should be focused on for statistical tests.

In this data set, which includes the website information of a company, there is information such as the number of advertisements that users see and click on, as well as earnings information from this. There are two separate data sets, the control and test groups. These datasets are in separate sheets of the ab_testing.xlsx excel. Maximum Bidding was applied to the control group and Average Bidding was applied to the test group.

Variables:

* Impression: Number of advertisement
* Click: Number of click on the displayed advertisement
* Purchase: Number of products purchased after the ads clicked
* Earning: Earnings after purchases
