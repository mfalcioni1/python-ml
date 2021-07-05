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

## Answers
1. No single classifier works best across multiple scenarios. (pg. 53)

2. It standardizings the continuous variables by subtracting the estimated mean and then dividing by the estimated standard deviation (normalization). (pg.56)

3. They use one-vs-all classification. (pg. 56)

4. Setting a learning rate too large will result in the algorithm overshooting the minima, too small will require more epochs until convergence making the learning especially slow for large datasets. (pg. 57)

5. Overfitting is when the model learns the patterns in the training data well, but fails to generalize for unseen data.

6. If the data values are not perfectly linearly separable, then the model will never converge.