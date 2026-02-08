## Lecture 3
### Regularization and Optimization

YouTube link to lecture video: https://www.youtube.com/watch?v=dyNGd06MWn4&list=PLoROMvodv4rOmsNzYBMe0gJY2XS8AQg16&index=3

- multi-dimensional array --> "tensor"
- Can't use series of if-else rules to classify images because of various problems, e.g. occlusion, intravariation, background content, etc. 
- Loss function tells us how good (bad) our current classifier is. If have x_i as image and y_i as label the loss over the dataset is an average of loss over examples. 
- Regularization: Data Loss + Regularization, where Data Loss measures the predictions vis-a-vis the training data and Regularization is a term that penalizes the model on the training data.  "Point of regularization is to do worse on the training data but better on the test/unseen data." 
- You don't want to overfit your data, e.g. have a line that runs through every point. Regularization discourages this. 
- Why regularize?
  - Express preference over weights
  - Make the model _simple_ so it works on test data
  - Improve optimization by adding curvature
- Softmax is great because it takes any set of floating point numbers and converts it to a probability distribution [NOTE: This looks like the MLE from statistical theory.] Converts list of numbers to probabilities. 
- How do we find the best W (regularization matrix)? Accomplish this with optimization.
  - Analogy is trying to find the lowest point in a landscape where the z-axis is elevation. 
- Strategies to find the best W:
  1. Assign random values. This is the worst option but will still outperform a baseline value. 
  2. Follow the slope. Fundamental way models trained in this course and way deep learning models are trained. In 1D, this is the derivative. In multiple dimensions, calculate the gradient (partial derivatives).
- Gradient descent: calculate the slope at each point on loss landscape and take direction downward.  