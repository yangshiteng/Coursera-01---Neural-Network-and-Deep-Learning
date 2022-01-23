# Week 1

- The term Deep Learning, refers to traiing Neural Networks, sometimes, very large Neural Networks
- Activation function: ReLU function (Rectified Linear Unit) f(x) = max(0,x)
![image](https://user-images.githubusercontent.com/60442877/150634901-65b2f692-e189-44b6-bdd0-8102312e8d12.png)
- Every input layer feature is interconnected with every hidden layer feature
- The  applications of deep learning today are online advertising, computer vision, speech recognition, machine translation, autonomous driving
- For image application, we usually use CNN (Convolutional Neural Network)
- For sequence data, like audio, we usually use RNN (Recurrent Neural Network)
- Structure Data: basically databases of data, each of the features has a very well defined meaning
- In contrast, unstructured data refers to things like audio, raw audio or images where you might want to recognize whats in the image. The features might be the pixel values in an image or the individual works in a piece of text.
- Why Deep Learning takes off in recent years:
![image](https://user-images.githubusercontent.com/60442877/150638453-04160287-a414-4e8a-a201-0e1fee5860ab.png)
![image](https://user-images.githubusercontent.com/60442877/150638473-a615d0a2-4652-4d9f-ae95-f9424dd47a88.png)
1. Deep learning has resulted in significant improvements in important applications such as online advertising, speech recognition, and image recognition. 
2. We have access to a lot more computational power.
3. We have access to a lot more data.
- One of the huge breakthroughs in Neural Networks is the switching from the sigmoid activation function to the ReLU activation function. And this switch make gradient descent worksd much faster 

![image](https://user-images.githubusercontent.com/60442877/150673774-ea8bf526-fead-40b5-8f43-5bc304346a2e.png)


# Week 2

- Logistic Regression is an algorithm for binary classification 
- Let's look at how an image is represented in a computer. To store an image, the computer stores three separater matrices corresponding to the red, green, and blue color channels fo this image. So, if your input image is 64x64 pixels, then, you would have 3 64x64 matrices corresponding to the red, green, and blue pixel intensity values for your images.
![image](https://user-images.githubusercontent.com/60442877/150640109-4bcb969d-3487-49aa-ad91-d3d57a92299b.png)
- So, to turn these pixel intensity values into a feature vector, we will unroll all of these pixel intensity values into an input feature vector x by rows from red, then green, to blue matrices. If the image is 64x64 pixels, then, the toal dimention of this feature vector is 3x64x64.
- In Python of Neural Networks and Deep Learning, the shape of X (traning or testing data) is nxm, where n is the dimension of feature vector and m is the number of data. So this type of setting in X is different from the traditional X. In the same way, the y (observation) is 1xm which is different from the traditional setting
- logistic function or sigmoid function can be used to help us transform the output value of a linear function into probability value
- Loss function, denoted by 'L', can measure how well you are doing on a single observation, for classification, the loss function is -log(p) in which, p is the predicted probability being the true label on that single observation, for regression, the loss function is the square of the residual
- Cost function, denoted by 'J', can measure how well you are doing on a whole traning dataset, the cost function is the average of the loss functions
- Vectorization will help you run your algrotihm way more faster than just for loop


