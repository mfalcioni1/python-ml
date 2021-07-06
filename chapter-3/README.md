# Additional Resources

[CMU Deep Learning Lecture Notes](https://sebastianraschka.com/pdf/lecture-notes/stat479ss19/)

# Active Learning

## Questions
1. What is "no free lunch theorem"?

2. How does `StandardScaler` in `sklearn` transform the dependent variables?

3. How do most algorithms in `sklearn` handle multi-classification problems?

4. Why is setting the appropriate learning rate for an algorithm important?

5. What is overfitting?

6. What is the biggest disadvantage of the perceptron algorithm?

7. What is the logit function?

8. What role does the logit function play in logistic regression?

9. What is the sigmoid function?

10. Why do we call it the "log-likelihood function"? What is the value of that transformation?

## Answers
1. No single classifier works best across multiple scenarios. (pg. 53)

2. It standardizings the continuous variables by subtracting the estimated mean and then dividing by the estimated standard deviation (normalization). (pg.56)

3. They use one-vs-all classification. (pg. 56)

4. Setting a learning rate too large will result in the algorithm overshooting the minima, too small will require more epochs until convergence making the learning especially slow for large datasets. (pg. 57)

5. Overfitting is when the model learns the patterns in the training data well, but fails to generalize for unseen data.

6. If the data values are not perfectly linearly separable, then the model will never converge.

7. The logit function takes input values in `[0, 1]` and transforms them to values of the entire real-number range. (pg. 61)

8. It allows us to express a linear relationship between independent variables and the log-odds (dependent discrete 0/1 variable). (pg. 61)

9. It is the inverse of the logit function that allows us to obtain predicted probabilities from our logistic regression model. It is characterized by its "S" shape, which is where it derives its name. The function is of the form `1/(1+ e(-z))` where `z` is the transpose of the weights vector multiplied by the feature vector. `w^Tx = w0x0 + w1x1 + ...` (pg. 62)

10. It is the "log-likelihood function" because we take the "log" of the likelihood function. This allows us to instead compute the derivative of a sum instead of a product. It offers an additional benefit in computing to help us avoid numeric underflow when likelihoods become very small. (pg. 65)