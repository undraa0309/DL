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


CustomMLP: loss and accurity 
![image](https://github.com/undraa0309/DL/assets/133347765/c10e6df4-9343-4e2a-9278-5b38eb332f2e)

















