```
Name : JEEVAGOWTHAM S
Roll no : 212222230053
Date : 13/08/2024
```
# EXPERIMENT 01- ARITHMETIC OPERATION AND LOGICAL OPERATION IN 8086


## Aim: 
  To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  
```python
org 100h
mov al,024h;
mov bl,al;
add bl,al;
mov [0123h],bl;
ret
```

## Output  
 ![image](https://github.com/user-attachments/assets/9653f400-407d-4296-9643-099e8e200611)

## Subtraction 
```python
org 100h
mov al,024h;
mov bl,[0123h+02];
sub bl,al;
mov [0123h+04],bl;
ret
```
## Output
![image](https://github.com/user-attachments/assets/38d763b8-2d07-4c36-af2f-632eef55a2d4)


## Multiplication
```python
org 100h
mov bx,0015h;
mov al,[bx];
mul bl;
mov [0015h+04],al;
ret
```
 ## Output  
![image](https://github.com/user-attachments/assets/46d9b340-ee73-47ea-bc1c-8380debe6fc9)



## Division
```python
org 100h
mov bx,0040h;
mov al,[bx+02];
div bl;
mov [0040h+04],al;
ret
```
## Output  
![image](https://github.com/user-attachments/assets/7367c348-161e-49ac-97e6-22c5ae023584)


## Programs for logical  operations

## AND
```python
org 100h
mov bx,1000h;
and bx,1111h;
mov [0040h+02],bx;
ret
```
## Output 
![image](https://github.com/user-attachments/assets/7b87ef54-f7dc-426a-b892-e9fbea7ceffc)

## OR
```python
org 100h
mov ax,[0040h+06];
mov bx,1000h;
or ax,bx;
mov [0040h+02],ax;
ret
```
## Output
![image](https://github.com/user-attachments/assets/5f690135-20d2-4cbf-81fd-fa86f9d70066)


## NOT
```python
org 100h
mov bx,0040h;
mov ax,[bx]; 
not al;
mov [0040h+04],ax;
ret
```
## Output
![image](https://github.com/user-attachments/assets/c6d52daa-1b6f-472c-946a-61773d4cd882)

## XOR
```python
org 100h
mov bx,0040h;
mov ax,[bx]; 
xor ax,bx;
mov [0040h+04],ax;
ret
```
## Output
![image](https://github.com/user-attachments/assets/b0a4ca28-d366-47c7-b65d-1c26c8232f5d)

## Result :
Thus, ALP for fundamental arithmetic and logical operations are executed successfully.








