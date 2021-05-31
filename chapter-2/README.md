# Additional Resources

[CMU Deep Learning Lecture Notes](https://sebastianraschka.com/pdf/lecture-notes/stat479ss19/)

# Active Learning

## Questions
1. What is the connection between McCulloch-Pitts (MCP) neuron and Frank Rosenblatt's perceptron learning rule?

2. Formally, what are the steps of the perceptron learning rule?

3. What is the constraint to for convergence of the perceptron?

4. What happens when the convergence constraint of the perceptron is not met?

5. What is One vs. All (OvA) or One vs. Rest (OvR) classification?

6. How does ADAptive Linear NEuron (Adaline) differ from the perceptron?

7. What is the Wodrow-Hoff rule?

8. What is the objective function?

9. Explain gradient descent.

10. What is batch gradient descent?

## Answers
1. The MCP neuron model is a simplification of the interconnectivity of the brain. Neurons in this model either fire or don't depending on the brain function. This is how the perceptron learning rule is coded. (pg20)

2. (pg23)
- Initialize weights to 0 or a small random number
- For each training example, x(i): 
    + compute y-hat 
    + update the weights based on a learning rate when necessary

3. The classes are linearly separable. (pg25)
[A proof can be found here](https://sebastianraschka.com/pdf/lecture-notes/stat479ss19/L03_perceptron_slides.pdf)

4. The weights will update endlessly unless we apply a maximum number of iterations to perform. (pg36)

5. OvA classification is a technique used for multi-class classification where you train a learner for each class. Each learner uses one class as the positive and the others as the negative. Then for prediction we pass our data through each model and use the classification with the highest likelihood. (pg31)

6. Both are single layer; however, Adaline illustrates how to define and minimize a continuous cost function. (pg36)

7. Weights are updated based on a linear activation function within the neurons. 

8. The cost function to be optimized during machine learning.

9. In order to update our weights, we take a step in the opposite direction of the gradient of our cost function.
    + The change in weight we apply in our update is the negative gradient multiplied by the learning rate
    + To compute the gradient, we calculate the partial derivative of the cost function with respect to each weight.
(pg38-39)

10. When the weight update is calculated for all examples in our training data instead of updating the weights incrementally after each training example.