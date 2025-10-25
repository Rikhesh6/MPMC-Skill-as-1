# MPMC-Skill Assessment I
## AIM
To write an assembly language program in 8051 to find the smallest number in an array of N elements using conditional jump instructions.


## APPARATUS REQUIRED

* Personal Computer with KEIL Software

---
#### Program

```
ORG 0000H          
MOV R0, #06H       
MOV R1, #30H       
MOV A, @R1         
MOV B, A          
DEC R0             
INC R1          
NEXT: MOV A, @R1    
CLR C               
SUBB A, B          
JC SMALL            
SJMP L2          
SMALL: MOV B, @R1   
L2: INC R1       
DJNZ R0, NEXT        
MOV 40H, B          
END

```


---

## OUTPUT IMAGE FROM KEIL SOFTWARE
<img width="310" height="286" alt="image" src="https://github.com/user-attachments/assets/50a6ae90-8772-4342-86bd-7708ef9a0bf8" />

<img width="1919" height="838" alt="image" src="https://github.com/user-attachments/assets/351f0134-2303-4b14-96eb-20364b77e6fc" />

<img width="299" height="284" alt="image" src="https://github.com/user-attachments/assets/0197278f-58e1-4387-a5f5-7a2ba3f39777" />




