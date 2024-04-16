#MNIST Classification - Deep learning assigment 

![image](https://github.com/undraa0309/DL/assets/133347765/19b4f748-91be-431f-95cd-aa59c691ebd7)
출처: https://blog.naver.com/laonple/220648539191

1. model.py


#Input 입력 이미지는 28X28
#Conv(C1)
#5x5 크기의 kernel 6개와 stride=1, convolutional layer
#입력 크기는 32x32x1 이고, 출력 크기는 28x28x6
#Subsampling(S2)
#2x2 크기의 kernel 6개와 stride=2, subsampling layer
#입력 크기는 28x28x6 이고, 출력 크기는 14x14x6
#Conv(C3)
#5x5 크기의 kernel 16개와 stride=1, convolution layer
#입력 크기는 14x14x6 이고, 출력 크기는 10x10x16
#Subsampling(S4)
#2x2 크기의 kernel 16개와 stride=2, subsampling layer
#입력 크기는 10x10x16 이고, 출력 크기는 5x5x16
#Conv(C5)
#5x5 크기의 kernel 120개와 stride=1, convolutional layer
#입력 크기는 5x5x16 이고, 출력 크기는 1x1x120

Layer (F6)
tanh 함수를 활성화 함수로 이용하는 fully-connected layer
입력 유닛은 120개 이고, 출력 유닛은 84개
Layer (F7)
RBF(Euclidean Radia Basis Function unit)를 활성화 함수로 이용하는 output layer
입력 크기는 84 이고, 출력 크기는 10


#LeNet-5 parameters:

![image](https://github.com/undraa0309/DL/assets/133347765/b907f97c-2750-4bd8-a7b7-1e31c4eeb99b)




#CustomMLP parameters:

![image](https://github.com/undraa0309/DL/assets/133347765/c0146c36-2c70-400d-ba78-3223957392f5)




2. main.py

LeNet5: loss and accurity 

![image](https://github.com/undraa0309/DL/assets/133347765/a701c860-c490-473a-a3e3-589d89cbe409)



















