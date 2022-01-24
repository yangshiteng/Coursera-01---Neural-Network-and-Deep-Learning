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
The cost function is the expectation of loss function, thus, in practice, it is the average of loss function in the training dataset

# Week 2

- Logistic Regression is an algorithm for binary classification 
- Let's look at how an image is represented in a computer. To store an image, the computer stores three separater matrices corresponding to the red, green, and blue color channels fo this image. So, if your input image is 64x64 pixels, then, you would have 3 64x64 matrices corresponding to the red, green, and blue (RGB) pixel intensity values for your images. To represent color images, the red, green and blue channels (RGB) must be specified for each pixel, and so the pixel value is actually a vector of three numbers ranging from 0 to 255.
![image](https://user-images.githubusercontent.com/60442877/150640109-4bcb969d-3487-49aa-ad91-d3d57a92299b.png)
![image](https://user-images.githubusercontent.com/60442877/150675287-43d1b9a8-7353-4966-922c-a76c7e2b16be.png)

- So, to turn these pixel intensity values into a feature vector, we will unroll all of these pixel intensity values into an input feature vector x by rows from red, then green, to blue matrices. If the image is 64x64 pixels, then, the toal dimention of this feature vector is 64x64x3.
- In Python of Neural Networks and Deep Learning, the shape of X (traning or testing data) is nxm, where n is the dimension of feature vector and m is the number of data. So this type of setting in X is different from the traditional X. In the same way, the y (observation) is 1xm which is different from the traditional setting
- logistic function or sigmoid function can be used to help us transform the output value of a linear function into probability value
- Loss function, denoted by 'L', can measure how well you are doing on a single observation, for classification, the loss function is -log(p) in which, p is the predicted probability being the true label on that single observation, for regression, the loss function is the square of the residual
- Cost function, denoted by 'J', can measure how well you are doing on a whole traning dataset, the cost function is the average of the loss functions
- Vectorization will help you run your algrotihm way more faster than just for loop

## Python Code to transform image data into one column vector

![image](https://user-images.githubusercontent.com/60442877/150675494-17479e7c-de1b-41f2-93ed-ee8906ed2c63.png)

## Normalization (with the numpy broadcasting technique)

![image](https://user-images.githubusercontent.com/60442877/150675622-bea915ab-2d2b-4d65-947f-12f230b32fa8.png)

![image](https://user-images.githubusercontent.com/60442877/150675715-8bcff823-af96-4f54-8e8d-192a02352ae1.png)

![image](https://user-images.githubusercontent.com/60442877/150675794-b35a29ac-18bd-44e0-bfa7-ec0ebc8895d8.png)

## SoftMax

![image](https://user-images.githubusercontent.com/60442877/150675871-acf524c2-adc7-4d43-a6d5-3b6a29c8b341.png)
![image](https://user-images.githubusercontent.com/60442877/150676043-33bd20fd-ec86-4cbb-8397-712c3a7814c2.png)
![image](https://user-images.githubusercontent.com/60442877/150676083-0c2f8ac9-c8d3-4d5e-8b13-28b1cbf74f41.png)


# Week 3

- When count the number of Neural Networks, we usually don't count input layer
- Use the ReLU activation function will make your Neural Networks way more faster than other types of activation function such as sigmoid function
- Never use sigmoid activation function except for the output layer of binary classification
- The most commonly used activation function is ReLU function
- Activation function types:
1. Sigmoid Function: f(x) = 1/(1+exp(-x))
2. Tanh Function: f(x) = (exp(x)-exp(-x))/(exp(x)+exp(-x))
3. ReLU function: f(x) = max(0,x)
4. Leaky ReLU function: f(x) = max(0.01x,x)
- All activation functions are Non-linear













