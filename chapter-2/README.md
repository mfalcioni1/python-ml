# Active Learning

## Questions
1. What is the connection between McCulloch-Pitts (MCP) neuron and Frank Rosenblatt's perceptron learning rule?

2. Formally, what are the steps of the perceptron learning rule?

3. What is the constraint to for convergence of the perceptron?

## Answers
1. The MCP neuron model is a simplification of the interconnectivity of the brain. Neurons in this model either fire or don't depending on the brain function. This is how the perceptron learning rule is coded. (pg20)

2. (pg23)
- Initialize weights to 0 or a small random number
- For each training example, x(i): 
    + compute y-hat 
    + update the weights based on a learning rate when necessary

3. The classes are linearly separable. (pg25)