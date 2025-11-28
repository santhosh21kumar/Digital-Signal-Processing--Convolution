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

n1=a+b:1:length (z)+a+b-1;

figure(3);

stem(n1,z);

xlabel('time');

ylabel('amplitude');

title('linear convolution');

## OUTPUT:
<img width="906" height="479" alt="Screenshot 2025-11-28 205151" src="https://github.com/user-attachments/assets/42f726e9-212b-407c-8980-804d5cd7cb26" />
<img width="905" height="486" alt="Screenshot 2025-11-28 205143" src="https://github.com/user-attachments/assets/d42691b8-e8e1-455e-a59e-c0c5cf9dfefe" />
<img width="909" height="479" alt="Screenshot 2025-11-28 205134" src="https://github.com/user-attachments/assets/a3c682ff-5378-4551-89f8-3a63dfaab6ef" />










## RESULT:
![WhatsApp Image 2025-11-28 at 13 02 06_2126dd0c](https://github.com/user-attachments/assets/92e0bf8b-0e7e-4acf-bd08-5e5ea626a4a8)



