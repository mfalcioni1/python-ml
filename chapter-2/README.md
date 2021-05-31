# Active Learning

## Questions
1. What is the connection between McCulloch-Pitts (MCP) neuron and Frank Rosenblatt's perceptron learning rule?

2. Formally, what are the steps of the perceptron learning rule?

## Answers
1. The MCP neuron model is a simplification of the interconnectivity of the brain. Neurons in this model either fire or don't depending on the brain function. This is how the perceptron learning rule is coded.

2. 
- Initialize weights to 0 or a small random number
- For each training example, [b]x[\b](i): 
    + compute y-hat 
    + update the weights based on a learning rate when necessary