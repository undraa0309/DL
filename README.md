#MNIST Classification - Deep learning assigment 

![image](https://github.com/undraa0309/DL/assets/133347765/19b4f748-91be-431f-95cd-aa59c691ebd7)
출처: https://blog.naver.com/laonple/220648539191

1. model.py


Input 입력 이미지는 28X28
Conv(C1)
5x5 크기의 kernel 6개와 stride=1, convolutional layer
입력 크기는 32x32x1 이고, 출력 크기는 28x28x6
Subsampling(S2)
2x2 크기의 kernel 6개와 stride=2, subsampling layer
입력 크기는 28x28x6 이고, 출력 크기는 14x14x6
Conv(C3)
5x5 크기의 kernel 16개와 stride=1, convolution layer
입력 크기는 14x14x6 이고, 출력 크기는 10x10x16
Subsampling(S4)
2x2 크기의 kernel 16개와 stride=2, subsampling layer
입력 크기는 10x10x16 이고, 출력 크기는 5x5x16
Conv(C5)
5x5 크기의 kernel 120개와 stride=1, convolutional layer
입력 크기는 5x5x16 이고, 출력 크기는 1x1x120

Layer (F6)
tanh 함수를 활성화 함수로 이용하는 fully-connected layer
입력 유닛은 120개 이고, 출력 유닛은 84개
Layer (F7)
RBF(Euclidean Radia Basis Function unit)를 활성화 함수로 이용하는 output layer
입력 크기는 84 이고, 출력 크기는 10


#LeNet-5 parameters:

       Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1            [-1, 6, 28, 28]             156
              Tanh-2            [-1, 6, 28, 28]               0
         AvgPool2d-3            [-1, 6, 14, 14]               0
            Conv2d-4           [-1, 16, 10, 10]           2,416
              Tanh-5           [-1, 16, 10, 10]               0
         AvgPool2d-6             [-1, 16, 5, 5]               0
            Linear-7                  [-1, 120]          48,120
              Tanh-8                  [-1, 120]               0
            Linear-9                   [-1, 84]          10,164
             Tanh-10                   [-1, 84]               0
           Linear-11                   [-1, 10]             850
          Softmax-12                   [-1, 10]               0
================================================================
Total params: 61,706
Trainable params: 61,706
Non-trainable params: 0
----------------------------------------------------------------
Input size (MB): 0.00
Forward/backward pass size (MB): 0.11
Params size (MB): 0.24
Estimated Total Size (MB): 0.35
----------------------------------------------------------------

#CustomMLP parameters:

----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Linear-1                   [-1, 64]          50,240
           Dropout-2                   [-1, 64]               0
              ReLU-3                   [-1, 64]               0
            Linear-4                   [-1, 64]           4,160
           Dropout-5                   [-1, 64]               0
              ReLU-6                   [-1, 64]               0
            Linear-7                   [-1, 64]           4,160
           Dropout-8                   [-1, 64]               0
              ReLU-9                   [-1, 64]               0
           Linear-10                   [-1, 32]           2,080
          Dropout-11                   [-1, 32]               0
             ReLU-12                   [-1, 32]               0
           Linear-13                   [-1, 16]             528
          Dropout-14                   [-1, 16]               0
             ReLU-15                   [-1, 16]               0
           Linear-16                   [-1, 16]             272
          Dropout-17                   [-1, 16]               0
             ReLU-18                   [-1, 16]               0
           Linear-19                   [-1, 10]             170
          Dropout-20                   [-1, 10]               0
             ReLU-21                   [-1, 10]               0
           Linear-22                   [-1, 10]             110
          Softmax-23                   [-1, 10]               0
================================================================
Total params: 61,720
Trainable params: 61,720
Non-trainable params: 0
----------------------------------------------------------------
Input size (MB): 0.00
Forward/backward pass size (MB): 0.01
Params size (MB): 0.24
Estimated Total Size (MB): 0.24
----------------------------------------------------------------



2. main.py

LeNet5: loss and accurity 

![image](https://github.com/undraa0309/DL/assets/133347765/a701c860-c490-473a-a3e3-589d89cbe409)



















