# MPMC-Skill Assessment I
## AIM
To write an assembly language program in 8051 to find the smallest number in an array of N elements using conditional jump instructions.


## APPARATUS REQUIRED

* Personal Computer with KEIL Software

---
#### Program

```
ORG 0000H          
MOV A, 20H        
MOV R0, A
MOV R1, #30H      
MOV A, @R1         
MOV B, A           
DEC R0             
INC R1          
NEXT: MOV A, @R1    
CLR C               
SUBB A, B           
JC SMALL            
SJMP SKIP           
SMALL: MOV B, @R1   
SKIP: INC R1        
DJNZ R0, NEXT       
MOV 40H, B          
END
```
---

## OUTPUT IMAGE FROM KEIL SOFTWARE
<img width="1919" height="861" alt="image" src="https://github.com/user-attachments/assets/e1bc6e66-8e5f-46f2-9744-ff9b383ca8df" />
<img width="318" height="293" alt="image" src="https://github.com/user-attachments/assets/17aca8a6-a2ed-4b0b-a2e1-d5903549ca90" />
<img width="309" height="288" alt="image" src="https://github.com/user-attachments/assets/79bc391e-22bb-436c-8282-40bfe490de51" />
<img width="311" height="283" alt="image" src="https://github.com/user-attachments/assets/b235f51a-5a67-4fb8-a2a7-309f97c811e1" />

---
## RESULT:
The smallest number in an array of N elements is found.






