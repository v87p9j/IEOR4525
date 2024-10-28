java c
IEOR4525 Fall 2021 Midterm
October 22, 2021
1 Linear regression (25 pts)
1.1 Assumptions of linear regression (6 pts)
List at least three different cases where applying linear regression directly would be problematic.
1.2 Linear regression with regularization (10 pts)
Consider a dataset {(xi, yi)}ni=1 where xi ∈ Rd and yi ∈ R, where d > 1. Suppose we have a regression model with parameters w ∈ Rd.
1. Ridge regression:

Write out the gradient of w.
Is there a closed form. solution for the optimal w∗? If so, please write out the expression of w∗; otherwise, explain why there isn’t.
2. Lasso regression:

Suppose we fix w at some value such that none of the elements are zero. Write out the gradient of w.
Is there a closed form. solution for the optimal w∗? If so, please write out the expression of w∗; otherwise, explain why there isn’t.
(Hint: In expressing the gradient of w, you may make use of the following pre-defined function:

)
1.3 Elastic net (9 pts)
You want to design a regressor with good prediction accuracy. Knowing that various kinds of regularization help, you decide to incorporate both the lasso and ridge penalties in the design of your optimization criterion. Given training data (x1, y1), . . . ,(xn, yn) (where each xi ∈ Rd and each yi ∈ R) you come up with the following optimization

where: (i) X is a d×n data matrix where the ith column corresponds to training data xi, (ii) y is a 1 × n output vector where the ith component corresponds to the training output yi, and (iii) w is a 1×d parameter weight vector. λ ≥ 0 and α ∈ [0, 1] are known trade-off parameters. Show that this optimization can be turned into a lasso regression by appropriately augmenting the training data.
2 Classification (15 pts)
2.1 5 pts
For each of the following classifiers, specify whether they are always a linear classifier or not:
1. LDA;
2. logistic regression;
3. QDA;
4. kNN;
5. Naive Bayes.
2.2 5 pts
Suppose data is sampled from the following distribution: The class y ∈ {0, 1} is equal to 1 with probability 0.5 and 0 with probability 0.5. Then given y, a single feature x is sampled from the Gaussian distribution N (y, σ2), where σ is the variance (note that the variance is shared across classes) and y is the mean. Recall that in class we define the Bayes classifier as the classifier that minimizes the probability of classifying incorrectly.
What is the Bayes decision boundary for this problem?
2.3 5 pts
Suppose that data is sampled from the following distribution: The class y ∈ {0, 1} is equal to 1 with probability 0.5 and 0 with probability 0.5. Then given y, two features x1, x2 are sampled, with x1 = y and x2 sampled from the standard Gaussian distribution N (0, 1).
Is 代 写IEOR4525 Fall 2021 MidtermC/C++
代做程序编程语言the Bayes decision boundary unique for this problem? If so, what is it? If not, describe the set of Bayes decision boundaries.
3 Logistic Regression (9pts)
Consider the logistic regression model y = g(βTx), where g(z) = 1+ez/ez is the logistic/sigmoid function. (Note that we omit the intercept, or, equivalently, enforcing the intercept to be zero.)
Suppose the weights are β = (− ln(4), ln(2), − ln(3)). A given data point has feature vector x = (1, 1, 1). What is the probability that this data point has a label of 1? (Please provide your answer in the form. of a fraction b/a.)
4 Naive Bayes (30 pts)
4.1 (15 pts)

Figure 1: Example data set
Suppose we have the two features with two binary-valued (i.e., boolean) vari-ables X1, X2 ∈ {0, 1} and label Y ∈ {0, 1}. In Figure 1 we show three positive samples (”+” for Y = 1 ) and one negative samples (”−” for Y = 0 ). Suppose we learn a Naive Bayes classifier from the examples in Figure 1, using MLE (maximum likelihood estimation) as the training rule.
1. Write down the prior probabilities P(Y ), and conditional probabilities P(Xi| Y = 0), P(Xi| Y = 1) for i = 1, 2. Note: both P(Y ) and P (Xi| Y ) should be Bernoulli distributions.
2. What will the predicted label be, if (x1, x2) = (1, 0) is provided as input to the trained classifier? Justify your answer.
4.2 (15 pts)
Recall that a Naive Bayes classifier with observed random variables Xi(i = 1, . . . , n) and the query variable Y uses the classification rule:

And a linear classifier uses the classification rule:

where x0 ≡ 1 is a bias feature.
Consider a Naive Bayes classifier with binary-valued features, i.e. xi ∈ {0, 1}. Prove that it is also a linear classifier, by defining weights wy,i (for i = 0, . . . , n) such that both decision rules above are equivalent. The weights should be expressed in terms of the Naive Bayes probabilities, i.e., P(y) and P (xi| y). You may assume that all the Naive Bayes probabilities are non-zero.
5 Bootstrap (21 pts)
Let’s suppose that we sample from an underlying distribution over the set of integers between 1 and 10 included, and we get the dataset {1, 2, 3, 10}. Suppose that we draw B bootstrap samples of size 4 from this dataset.
For all the questions, clearly explain your reasoning.
1. (5 pts) What is the expected number of occurrences of the value 1 in a given bootstrap sample?
2. (5 pts) What is the probability that we get a bootstrap sample with more than one occurrence of 1?
3. (5 pts) What is the probability that we never draw a 2 in the B samples?
4. (6 pts) Explain how we could determine the variability of estimating the mean of the underlying data-generating process using the B bootstrap samples.





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
