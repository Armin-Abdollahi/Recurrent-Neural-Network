# Recurrent-Neural-Network
Recurrent Neural Network (RNN)

![RNN](/RNN.png)

A Recurrent Neural Network (RNN) is a class of artificial neural networks where connections between nodes form a directed graph along a temporal sequence. This allows it to exhibit temporal dynamic behavior for a time sequence. Unlike feedforward neural networks, RNNs can use their internal state (memory) to process sequences of inputs. This makes them suitable for tasks like speech recognition or language modeling.

A brief overview of RNNs:

- Memory: RNNs have loops in them, allowing information to persist. In other words, RNNs have a memory that captures information about what has been calculated so far. This is crucial in tasks where context is important, such as language translation.
Backpropagation Through Time (BPTT): To train RNNs, a technique called BPTT is used, where the network is unfolded through time and the error is backpropagated through these unfolded steps.

- Challenges: RNNs are prone to short-term memory due to issues like vanishing and exploding gradients. This happens because, in the process of backpropagation, gradients can end up being multiplied by the weight matrix (which has small or large values) many times, leading to very small or very large gradients.

- Long Short-Term Memory (LSTM): To overcome these challenges, LSTMs, a special kind of RNN, were developed. They have a different structure that includes gates to control the flow of information, which helps in preserving the error that can be backpropagated through time and layers.

- Applications: RNNs are used in a variety of applications where sequential data is involved, such as text generation, machine translation, and voice recognition.


RNNs are powerful because they combine two properties: they can process sequences of variable length, and they have a modular structure that can be used to build more complex architectures like LSTMs or Gated Recurrent Units (GRUs).
