# FACTORIAL-OF-A-NUMBER-USING-8051-KEIL

**AIM:**

To write and execute Assembly language Program to perform factorial of a number using 8051 keil.
APPARATUS REQUIRED: Personal computer with Keil software

**ALGORITHM:**

• Start  

• Input: Read the number n.  

• Initialize:  

•Set factorial to 1.  

•Set i to 1.  

• Loop: While i is less than or equal to n:  

•Multiply factorial by i.  

•Increment i by 1.  

• Output: Store or print the value of factorial.  

• End

**FLOW CHART:**
<img width="261" height="308" alt="image" src="https://github.com/user-attachments/assets/bffe89f6-3ba9-4294-b817-8b545f680e66" />

**Program:**

ORG 0000H   

MOV A,#04H  

MOV R0,A  

ACALL FACTORIAL  

MOV 40H,A  

SJMP THIN  

FACTORIAL:DEC R0  

CJNE R0,#01H,PRODUCT  

SJMP THICK   

PRODUCT:MOV B,R0  

MUL AB  

ACALL FACTORIAL  

THICK: RET  

THIN:  

END

### Output:
![WhatsApp Image 2025-10-28 at 11 06 39_1f8400a7](https://github.com/user-attachments/assets/0a4aa0b2-12aa-42cf-9898-4c63cfa85eb7)


### Manual Calculations:
![WhatsApp Image 2025-10-28 at 11 08 54_0657a7e9](https://github.com/user-attachments/assets/4f2bd031-ec11-4af3-ae24-743e78340344)


### Result:

Thus the factorial of a number using 8051 keil was calculated and shown the output.
