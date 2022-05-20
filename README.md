# Digit-Recognizer-with-MNIST-data

Hi, in this repository I have made a Digit Recognizer System using the traditional MNIST data. I have implemented it using two approaches.
1. Creating a deep neural network using Keras API
2. Creating a Convolutional Neural Network using Functional API


Both my submissions got a decent score in Kaggle Digit Recognizer Competition a score of 98.25 for first submission and a score of 99.025 for second submission.

My main motto for creating this repository is to show why we need to implement CNN for Computer Vision instead of Deep Neural Network although both worked pretty well for this dataset. So,lets observe both models 
In model 1 the number of parameters is enormous 5lakh parameters whereas in model2 I used only 50k parameters and even managed to get slightly better accuracy. 
The drawbacks of traditional Deep Neural Network comes from the fact that parameters are not being shared among all other neurons. Lets say our weights are trained in such a way that we got vertical edge detector in our neural network and the paramers of filter also be able to detect vertical edges. As we are convolving the filter on the entire image it means that paramters get shared and be useful to detect all vertical edges from the image. Whereas in a Neural Network the parameters learnt from that input neurons only are shared by it and do not get shared with other neurons in the network. So, we have to make model so deep so as to get parameters learnt by some neurons to be propagated to entire image. 
Second drawback comes due to Deep Neural Networks being computationally more expensive than Convolutional Neural Networks which is a bad signature because we often need to have models having enormous number of features and training data. If our parameters also become enormous it would take much more time to run. 


So thats why we need to prefer CNN for any computer vision task over deep neural nets
