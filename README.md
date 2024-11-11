# EXPERIMENT 01- ARITHMETIC OPERATION AND LOGICAL OPERATION IN 8086
```
Name : NAVEEN KUMAR B
Roll no : 212222230091
Date : 13/08/2024
```


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
8. <img src="https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png" width=50%>
  
10.	Click on emulate to start emulation 
<img src="https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png" width=50%>

11. If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 
<img src="https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png" width=10%>


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
<img src="https://github.com/user-attachments/assets/34adf8b5-9c1e-4d57-8184-466d359d77f4" width=50%>

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
<img src="https://github.com/user-attachments/assets/5589247f-3239-48b8-8b71-d45f0a1df8b8" width=50%>

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
 <img src="https://github.com/user-attachments/assets/28705677-66b6-48eb-a8e9-0a3eeeb8fcff" width=50%>

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
<img src="https://github.com/user-attachments/assets/85e6271d-2fc4-4839-b6d3-7e5cac607173" width=50%>

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
<img src="https://github.com/user-attachments/assets/35411f82-ec16-48fc-b1bd-85c963d050cd" width=50%>

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
<img src="https://github.com/user-attachments/assets/ee488f35-b632-44e5-b858-13d69cbd1ff7" width=50%>

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
<img src="https://github.com/user-attachments/assets/54cca62e-f8a5-4274-beb2-c4e5abecbd10" width=50%>

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
<img src="https://github.com/user-attachments/assets/d3280d78-31cc-4ab7-919e-7fa8099c4ca2" width=50%>

## Result :
Thus, ALP for fundamental arithmetic and logical operations are executed successfully.








