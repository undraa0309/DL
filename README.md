###MNIST Classification - Deep learning assigment 

![image](https://github.com/undraa0309/DL/assets/133347765/19b4f748-91be-431f-95cd-aa59c691ebd7)
출처: https://blog.naver.com/laonple/220648539191

1. model.py

LeNet- 5 

Input 입력 이미지는 28X28
 C1 (5*5*1+1)*6 = 156
 S2 AvgPool
 C3 (5*5*6+1)*16 = 2416
 S4
 C5 (16*5*5+1)*120 = 48120
OUTPUT (84+1)*10 = 850
        Total number of parameters = 123,412
        156+2,416+48,120+10,164+850 = 61,706
        backpropagation 61,706


#LeNet-5 parameters:

![image](https://github.com/undraa0309/DL/assets/133347765/b907f97c-2750-4bd8-a7b7-1e31c4eeb99b)




#CustomMLP parameters:

![image](https://github.com/undraa0309/DL/assets/133347765/c0146c36-2c70-400d-ba78-3223957392f5)




2. main.py

LeNet5: loss and accurity 

![image](https://github.com/undraa0309/DL/assets/133347765/f2bf8d5c-74c8-4132-a6e1-bf942eb53c17)

train_losses = [0.3111, 0.1059, 0.0691, 0.0481, 0.0354, 0.0264, 0.0183, 0.0129, 0.0082, 0.0054]
test_losses = [0.1289, 0.0960, 0.0776, 0.0691, 0.0686, 0.0732, 0.0634, 0.0748, 0.0622, 0.0689]
train_accuracies = [90.83, 96.76, 97.82, 98.49, 98.86, 99.19, 99.47, 99.61, 99.78, 99.90]
test_accuracies = [95.94, 96.79, 97.55, 97.88, 97.87, 97.73, 98.21, 97.91, 98.24, 98.15]


CustomMLP: loss and accurity 
![image](https://github.com/undraa0309/DL/assets/133347765/c10e6df4-9343-4e2a-9278-5b38eb332f2e)

train_losses = [0.3111, 0.1059, 0.0691, 0.0481, 0.0354, 0.0264, 0.0183, 0.0129, 0.0082, 0.0054]
test_losses = [0.1289, 0.0960, 0.0776, 0.0691, 0.0686, 0.0732, 0.0634, 0.0748, 0.0622, 0.0689]
train_accuracies = [90.83, 96.76, 97.82, 98.49, 98.86, 99.19, 99.47, 99.61, 99.78, 99.90]
test_accuracies = [95.94, 96.79, 97.55, 97.88, 97.87, 97.73, 98.21, 97.91, 98.24, 98.15]


3. LeNet -5 and Custom MLP 비교

![image](https://github.com/undraa0309/DL/assets/133347765/381b1b89-e83d-47cb-b91a-20ea2de904e3)


![image](https://github.com/undraa0309/DL/assets/133347765/83c717a9-f24a-4f33-8dbe-be79779bcb8f)


















