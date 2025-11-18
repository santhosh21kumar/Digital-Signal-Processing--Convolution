# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows
% INPUT SEQUENCE
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
% IMPULSE SEQUENCE
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response')
% LINEAR CONVOLUTION
z=conv2(x,y);
n1=a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title( 'linear convolution');


## OUTPUT:
<img width="1683" height="877" alt="Screenshot 2025-10-06 085114" src="https://github.com/user-attachments/assets/9b8f7edb-5a57-4a64-b217-55790c6d815a" />
<img width="1647" height="889" alt="Screenshot 2025-10-06 085230" src="https://github.com/user-attachments/assets/783c6726-848b-4a48-9d59-5a0b534f8a39" />
<img width="1703" height="879" alt="Screenshot 2025-10-06 085257" src="https://github.com/user-attachments/assets/ee95ef1f-12a6-40a9-b529-45174e2db4b5" />





## RESULT:
{6.4,17.8,5.7,-14.7,-43.6,55.8,7.2,47.1,60.2,-8.3,-1.7,23.7,15.2}
