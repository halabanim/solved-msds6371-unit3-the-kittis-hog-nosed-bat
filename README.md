Download Link: https://assignmentchef.com/product/solved-msds6371-unit3-the-kittis-hog-nosed-bat
<br>



<ol>

 <li>The world’s smallest mammal is the bumblebee bat, also known as the Kitti’s hog nosed bat. Such bats are roughly the size of a large bumblebee!  Listed below are weights (in grams) from a sample of these bats.  Test the claim that these bats come from the same population having a mean weight equal to 1.8 g. <em> (Beware: This data is <strong>NOT</strong> the same as in the lecture slides!)</em></li>

</ol>

Sample: 1.7   1.6    1.5    2.0    2.3    1.6    1.6    1.8    1.5    1.7   1.2    1.4    1.6    1.6    1.6

<strong> </strong>

<ol>

 <li>Perform a complete analysis using SAS. Use the six step hypothesis test with a conclusion that includes a statistical conclusion, a confidence interval, and a scope of inference (as best as can be done with the information above … there are many correct answers given the vagueness of the description of the sampling mechanism).</li>

 <li>Inspect and run this R Code and compare the results (t statistic, p-value, and confidence interval) to those you found in SAS. To run the code, simply copy and paste the below code into R.</li>

</ol>

<strong><em>sample = c(1.7, 1.6, 1.5, 2.0, 2.3, 1.6, 1.6, 1.8, 1.5, 1.7, 1.2, 1.4, 1.6, 1.6, 1.6)</em></strong>

<strong><em>t.test(x=sample, mu = 1.8, conf.int = “TRUE”, alternative = “two.sided”)</em></strong>

<ol start="2">

 <li>In the United States, it is illegal to discriminate against people based on various attributes. One example is age.  An active lawsuit, filed August 30, 2011, in the Los Angeles District Office is a case against the American Samoa Government for systematic age discrimination by preferentially firing older workers. Though the data and details are currently sealed, suppose that a random sample of the ages of fired and not fired people in the American Samoa Government are listed below:</li>

</ol>

<strong>Fired</strong>

34 37 37 38 41 42 43 44 44 45 45 45 46 48 49 53 53 54 54 55 56

<strong>Not fired</strong>

27 33 36 37 38 38 39 42 42 43 43 44 44 44 45 45 45 45 46 46 47 47 48 48 49 49 51 51 52 54




<ol>

 <li>Perform a permutation test to test the claim that there is age discrimination. Provide the Ho and Ha, the p-value, and full statistical conclusion, including the scope (inference on population and causal inference). Note: this was similar to an example in Live Session 1. You may start from scratch or use the sample code and PowerPoints from Live Session 1.</li>

 <li>Now run a two sample t-test appropriate for this scientific problem. (Use SAS.) <em>(Note: we may not have talked much about a two-sided versus a one-sided test. If you would like to read the discussion on pg. 44 (Statistical Sleuth), you can run a one-sided test if it seems appropriate.  Otherwise, just run a two-sided test as in class.  There are also examples in the Statistics Bridge Course.)</em> Be sure to include all six steps, a statistical conclusion, and scope of inference.</li>

 <li>Compare this p-value to the randomized p-value found in the previous sub-question.</li>

 <li>The jury wants to see a range of plausible values for the difference in means between the fired and not fired groups. Provide them with a confidence interval for the difference of means and an interpretation.</li>

 <li>Given the sample standard deviations from SAS, calculate by hand

  <ol>

   <li>Pooled standard deviation (s<sub>p</sub>)</li>

   <li>The standard error of ()</li>

  </ol></li>

 <li>Inspect and run this R Code and compare the results (t statistic, p-value, and confidence interval) to those you found in SAS. To run the code, simply copy and paste the code below into R.</li>

</ol>

<strong><em>Fired = c(34, 37, 37, 38, 41, 42, 43, 44, 44, 45, 45, 45, 46, 48, 49, 53, 53, 54, 54, 55, 56)</em></strong>

<strong><em>Not_fired = c(27, 33, 36, 37, 38, 38, 39, 42, 42, 43, 43, 44, 44, 44, 45, 45, 45, 45, 46, 46, 47, 47, 48, 48, 49, 49, 51, 51, 52, 54)</em></strong>

<strong><em>t.test(x = Fired, y = Not_fired, conf.int = .95, var.equal = TRUE, alternative = “two.sided”)</em></strong>

<em> </em>

<ol start="3">

 <li>In the last homework, it was mentioned that a Business Stats professor here at SMU polled his class and asked students them how much money (cash) they had in their pockets at that very moment. The idea was that we wanted to see if there was evidence that those in charge of the vending machines should include the expensive bill / coin acceptor or if it should just have the credit card reader. However, another professor from Seattle University was asked to poll her class with the same question.  Below are the results of the polls.</li>

</ol>

<strong>SMU</strong>

34, 1200, 23, 50, 60, 50, 0, 0, 30, 89, 0, 300, 400, 20, 10, 0

<strong>Seattle U</strong>

20, 10, 5, 0, 30, 50, 0, 100, 110, 0, 40, 10, 3, 0




<ol>

 <li>Run a two sample t-test to test if the mean amount of pocket cash from students at SMU is different than that of students from Seattle University. Write up a complete analysis: all 6 steps including a statistical conclusion and scope of inference (similar to the one from the PowerPoint). (This should include identifying the Ho and Ha as well as the p-value.)  Also include the appropriate confidence interval.  <strong>FUTURE DATA SCIENTIST’S CHOICE!: YOU MAY USE SAS<em> <u>OR</u></em> R TO DO THIS PROBLEM!</strong></li>

 <li>Compare the p-value from this test with the one you found from the permutation test from last week. Provide a short 2 to 3 sentence discussion on your thoughts as to why they are the same or different.</li>

</ol>

<ol start="4">

 <li>Calculate the estimate of the pooled standard deviation from the Samoan discrimination problem (see data from question 2). Use this estimate to build a power curve. Assume we would like to be able to detect effect sizes between 0.5 and 2 and we would like to calculate the sample size required to have a test that has a power of .8.  Simply cut and paste your power curve and SAS code.   HINT: USE THE CODE FROM DR. McGEE’s lecture. Instead of using <strong>groupstddevs</strong>, use <strong>stddev</strong> since we are using the pooled estimate.</li>

</ol>




<ol>

 <li>Now suppose we decided that we may be able to live with slightly less power if it means savings in sample size. Provide the same plot as above but this time calculate curves of sample size (y-axis) vs. effect size (.5 to 2) (x axis) for power = 0.8, 0.7, and 0.6.  There should be three plots on your final plot.  Simply cut and paste your power curve and SAS code.  HINT: USE THE CODE FROM DR. McGEE’s lecture. Instead of using <strong>groupstddevs</strong>, use <strong>stddev</strong> since we are using the pooled estimate. The effect size here refers to a difference in means, though there are many effect size metrics, such a Cohen’s D.</li>

</ol>




<ol>

 <li>Using similar code, estimate the savings in sample size from a test aimed at detecting an effect size of 0.8 with a power of 80% versus a power of 60%.</li>

</ol>

Note: You will learn how to do this in R in a future HW!