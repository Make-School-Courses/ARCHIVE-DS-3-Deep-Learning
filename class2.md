## Class 2: Activation functions

### Pre-work

- Read Ivan Vasilev’s [Deep Learning Tutorial: From Perceptrons to Deep Networks](https://www.toptal.com/machine-learning/an-introduction-to-deep-learning-from-perceptrons-to-deep-networks), but stop when you get to the Autoencoders section because it’s not relevant for this course.

### Topics

- Combining threshold with weights to create a single parameter vector including a bias
- Activation functions: sigmoid curves
- Perceptron learning rule, adjusting weights using gradient descent on error function

### Resources

- Watch Alexander Ihler’s videos on [Neural Networks](https://www.youtube.com/watch?v=bH6VnezBZfI) and [Gradient Descent](https://www.youtube.com/watch?v=WnqQrPNYz5Q).
- Read Mark Humphry’s notes on [Multi-layer Neural Networks](http://computing.dcu.ie/~humphrys/Notes/Neural/multi.neural.html).
- Read Andrew Trask’s articles: [A Neural Network in 11 Lines of Python (part 1: Optimization)](http://iamtrask.github.io/2015/07/12/basic-python-network/) and [A Neural Network in 13 Lines of Python (part 2: Gradient Descent)](http://iamtrask.github.io/2015/07/27/python-network-part2/). Pay close attention to the diagrams in part 2 to gain an intuition for gradient descent.
- Play around with the [TensorFlow Playground](http://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.30035&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false) to create multilayer perceptron networks.
- Read Nahua Kang article: [Multi-Layer Neural Networks with Sigmoid Function— Deep Learning for Rookies(2)](https://towardsdatascience.com/multi-layer-neural-networks-with-sigmoid-function-deep-learning-for-rookies-2-bf464f09eb7f).
- Watch Oscar Alsing video on [The Perceptron Made SIMPLE! Easiest way to UNDERSTAND the Perceptron!](https://www.youtube.com/watch?v=wL2aVUjDdoo).
- Watch The Coding Train videos on [10.2: Neural Networks: Perceptron Part 1 - The Nature of Code](https://www.youtube.com/watch?v=ntKn5TPHHAk).

### Challenges

- Augment your Perceptron class with the follow additional features:
    - Add a nonlinear sigmoid activation function (for example, the logistic function)
    - Implement `fit(X, y)`: train the weights and threshold using the perceptron learning rule until they converge (change by less than 0.0001 after one epoch)
    - Add a learning rate to control how fast the weights are updated in each iteration
    - Train your Perceptron on small 2-dimensional datasets like the examples from class. Compare the `weights` it found to your own (plotting makes this comparison really easy).
    - Train your Perceptron on the Iris dataset using one-versus-many encoding of classes (make a dummy boolean feature for each iris class, and then train on only one at a time). Plot the decision boundaries of each trained Perceptron along with the iris data itself.
