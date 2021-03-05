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

**Second Layer:**

Then the LeNet-5 applies average pooling layer or sub-sampling layer with a filter size 2×2 and a stride of two. The resulting image dimensions will be reduced to 14x14x6.

![image](https://user-images.githubusercontent.com/63854149/110180300-8e3f2e00-7e2f-11eb-91ce-48a55927ce62.png)

**Third Layer:**

Next, there is a second convolutional layer with 16 feature maps having size 5×5 and a stride of 1. In this layer, only 10 out of 16 feature maps are connected to 6 feature maps of the previous layer as shown below.

![image](https://user-images.githubusercontent.com/63854149/110180345-9bf4b380-7e2f-11eb-9745-adfc90d1bde5.png)

**Fourth Layer:**

The fourth layer (S4) is again an average pooling layer with filter size 2×2 and a stride of 2. This layer is the same as the second layer (S2) except it has 16 feature maps so the output will be reduced to 5x5x16.

![image](https://user-images.githubusercontent.com/63854149/110180418-c0509000-7e2f-11eb-9332-1ec905d58a5a.png)

**Fifth Layer:**

The fifth layer (C5) is a fully connected convolutional layer with 120 feature maps each of size 1×1. Each of the 120 units in C5 is connected to all the 400 nodes (5x5x16) in the fourth layer S4.

![image](https://user-images.githubusercontent.com/63854149/110180450-cd6d7f00-7e2f-11eb-9fa1-a608f3a41a8f.png)

**Sixth Layer:**

The sixth layer is a fully connected layer (F6) with 84 units.

![image](https://user-images.githubusercontent.com/63854149/110180481-dbbb9b00-7e2f-11eb-81d0-ff1f95ba29af.png)

**Output Layer:**

Finally, there is a fully connected softmax output layer ŷ with 10 possible values corresponding to the digits from 0 to 9.

![image](https://user-images.githubusercontent.com/63854149/110180501-e8d88a00-7e2f-11eb-83e6-7649f74aaf64.png)

**Summary of LeNet-5 Architecture**

![image](https://user-images.githubusercontent.com/63854149/110180522-f5f57900-7e2f-11eb-915c-508940b3362b.png)
