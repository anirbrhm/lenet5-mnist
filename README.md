# lenet5-mnist
Using LeNet-5 Deep Learning Architecture to classify handwritten digits

Using LeNet-5 architecture to classify the digits in the MNIST data-set is the "Hello World" of deep learning. 
Yann LeCun, Leon Bottou, Yosuha Bengio and Patrick Haffner proposed a neural network architecture for handwritten 
and machine-printed character recognition in 1990’s which they called LeNet-5. The architecture is straightforward 
and simple to understand that’s why it is mostly used as a first step for teaching Convolutional Neural Network.

![image](https://user-images.githubusercontent.com/63854149/110180078-25f04c80-7e2f-11eb-8287-4662e7093dd3.png)

**First Layer:**

The input for LeNet-5 is a 32×32 grayscale image which passes through the first convolutional layer with 6 feature maps 
or filters having size 5×5 and a stride of one. The image dimensions changes from 32x32x1 to 28x28x6.

![image](https://user-images.githubusercontent.com/63854149/110180230-651e9d80-7e2f-11eb-870c-b083951097a5.png)

