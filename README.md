This project uses deep learning to predict the categories of images in the Fashion MNIST dataset.

The idea originated while I was still modeling. Most of my regular clients were ecommerce fashion retailers, and some of them had issues with products being mislabeled on their website.  Often items would end up in the wrong category: men’s items would appear under women’s, a shirt would end up in the dresses section, a pair of red pants would be labeled as blue. If a customer searches the site for red pants, they won’t find that pair!

After all the hard work the creative team and I did around styling, modeling, photographing, and editing the images of these products, it was absolutely maddening when they didn’t end up in the right place on the company’s website. I asked around and discovered that humans were responsible for manually catching these errors - and with sometimes tens of thousands of new products being added to a site per day, it’s no wonder mistakes happened.

I’d been really enjoying reading about fun projects using computer vision using convolutional neural networks, and this seemed like a practical business application of the technology. Could I train a neural net to classify the images better than a human? Or at least flag suspiciously labeled images, so a human could do a quick review of this smaller subset of images. I realize a deep learning project is a big undertaking as a first project, but I’m excited about solving a real world business problem, so here goes!

I found two fashion image datasets that are good approximations of the type of images ecommerce fashion retailers use. I’ll start with the Fashion MNIST.

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
