## Lecture 2
YouTube link to lecture video: https://www.youtube.com/watch?v=pdqofxJeBN8&list=PLoROMvodv4rOmsNzYBMe0gJY2XS8AQg16&index=3

- An image is made up of a matrix of numbers, i.e. a "tensor of integers" between [0,255]. 
- Machine Learning: Data Driven Approach 
  - Collect a dataset of images and labels
  - Use machine learning algorithms to train a classifier
  - Evaluate classifier on new images
- Nearest Neighbor Classifier:
  - Train function: memorize all data and labels
  - Predict function: predict label of most similar image
  - Build classifiers that are fast at prediction. OK if they are slow during training. 
  - Must consider hyperparameters, too (hyperparamaters are choices about algorithms themselves). This is problem and dataset dependent so must try them out to see what works best. 
    - What is the best value of k to use? 
    - What is the best distance to use? L1 (Manhattan) or L2 (Euclidean?) 
    - Best way to select hyperparameters is to split the data into TRAIN, VALIDATE, and TEST sets then tune the hyperparameters on the VALIDATION set then evaluate with the TEST set. 
    - Cross-validation recommended for smaller datasets. 
  - kNN with pixel distance is never used since distance metrics on pixels are not informative. 
- Linear Classifier
  - Most important building block for all of machine learning
  - Parametric approach
  - The linear classifiers build together into neural networks
  - Loss (Object) function: Quantifies our "unhappiness" with the scores across the training data
    - Need to find a way to efficiently find the parameters that minimize the loss function ("optimization")
    - Softmax Classifier (multinomial logistic regression): interpret raw classifier scores as probabilities 
      - Goal is to maximize the probability of the sample belonging to the right class
