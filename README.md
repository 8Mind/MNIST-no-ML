# simple-MNIST
A simple way of inference for MNIST data that is 96.91% accurate.

# How does it work?
Each image lies in a vector space of dimension 28*28. 
The distance between two vectors (i.e. images) is given by the Euclidean norm of the difference vector.
So given a *test* image (one of 10,000), find it's 'distance' to all train images (60,000 many) and extract the train image which is closest.
Finally, assign the label of this train image as the prediction for the test image.
This classfifies 9,691/10,000 test images correctly.
