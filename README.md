# EXPERIMENT--01-ALP-FOR-8086
Name :MAHALAKSHMI.K

Roll no:212222240057


## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
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

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output 

<img width="2559" height="1599" alt="1" src="https://github.com/user-attachments/assets/d71a79ad-81cd-48f8-a369-57870bce26cd" />

 
## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT      


```
 
## Output  

<img width="2555" height="1599" alt="2" src="https://github.com/user-attachments/assets/5f451438-7c0e-476c-b2e9-056f924994a1" />


## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  
 
<img width="2557" height="1599" alt="3" src="https://github.com/user-attachments/assets/b5b61ed4-316f-4bfe-91cd-1a83465a6418" />


## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  

<img width="1028" height="630" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/c86f93fb-8fc9-4603-a67e-96b9463a809e" />


LOGICAL OPERATIONS
TRUTH TABLE FOR LOGICAL OPERATIONS

AND 
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```

OUTPUT:

<img width="1012" height="620" alt="Screenshot (5)" src="https://github.com/user-attachments/assets/052fd81d-4fc8-40c8-93bf-9eac283f0e54" />

OR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
Output:

<img width="991" height="634" alt="Screenshot (6)" src="https://github.com/user-attachments/assets/547f9ef8-e5b4-45c0-a729-db53b2024ff0" />

NAND alp:
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```

OUTPUT

<img width="1032" height="639" alt="Screenshot (7)" src="https://github.com/user-attachments/assets/53969f63-9804-4761-84a7-de00cf194a0a" />

NOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

OUTPUT

<img width="1031" height="638" alt="Screenshot (8)" src="https://github.com/user-attachments/assets/1fe0a4ad-fd3c-4069-817e-f6ab6d32a213" />

NOT alp
```
MOV AX,[3001H]
MOV BX,[3003H]
NOT AX
MOV [3005H],AX
HLT
```
OUTPUT

<img width="1036" height="638" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/b517cac6-222e-4e72-aa41-b4cd8aef5254" />

XOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```

OUTPUT



XNOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

output

<img width="1038" height="639" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/f6c2e15d-6f74-498e-b914-f10ae5622b85" />


## Result :
 Thus, a program is executed on ALP for the fundamental arithmetic and logical operations.








