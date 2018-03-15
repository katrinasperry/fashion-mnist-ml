# Fashion_MNIST

This project uses deep learning to predict the categories of images in the Fashion MNIST dataset. 

## Data
Similar to the MNIST dataset, the Fashion MNIST dataset contains a training set of 60,000 examples, and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes.

### Labels:
Each training and test example is assigned to one of the following labels:

0 T-shirt/top

1 Trouser

2 Pullover

3 Dress

4 Coat

5 Sandal

6 Shirt

7 Sneaker

8 Bag

9 Ankle boot 


## Measuring success
Accuracy will be the measure of success: 

number of correctly predicted images / total number of images

### Baseline accuracies for comparison
Support Vector Machine (svmRadial)
91%/87% - the one to beat!

Gradient Boosting Machine (gbm)
90%/85%

Neural Network (multinom)
84%/78%

LogitBoost
81%/75%

Baseline Algorithm (always predicts the most frequently occurring clothing item)
12%/10%

## References
[Fashion-MNIST](https://www.kaggle.com/zalando-research/fashionmnist)

[Deep Learning with Python](https://www.manning.com/books/deep-learning-with-python)

## Author
Katrina Sperry https://katrinasperry.github.io
