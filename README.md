# 8-Bit-Arithmetic-Operations-Using-8051

## Aim:
To perform 8-bit arithmetic operations such as addition, subtraction, multiplication, and division using the 8051 microcontroller.

## Apparatus Required:

•	Laptop with Keil uVision software

## Algorithm:

## For Addition:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Add the contents of registers A and B.
4.	Store the result in memory location 40H.
5.	Store the carry (if any) in 41H.

## Program:

      MOV A,30H;
      ADD A,31H;
      MOV 40H,A;
      JNC NEXT ;
      MOV 41H,#01H;
      SJMP END_PROGRAM;
      NEXT:MOV 41H,#00H;
      END_PROGRAM:NOP;
      END

## Output:

![WhatsApp Image 2025-10-27 at 13 49 05_5ff265f3](https://github.com/user-attachments/assets/0a238540-3e58-40ef-ad37-756b055c84f1)

![WhatsApp Image 2025-10-27 at 13 49 59_27ebcf06](https://github.com/user-attachments/assets/b190c8a5-c486-4fff-ad8c-0f323d0df44e)

![WhatsApp Image 2025-10-27 at 13 50 16_43ea44d1](https://github.com/user-attachments/assets/101c93f9-071f-45b9-a297-8ea5495da8cc)

## For Subtraction:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Subtract B from A.
4.	Store the result in memory location 40H.

## Program:

      ORG 0000H
      MOV A,30H
      SUBB A,31H
      MOV 40H,A
      JNC NEXT 
      MOV 41H,#01H;
      SJMP END_PROGRAM;
      NEXT:MOV 41H,#00H;
      END_PROGRAM:NOP;
      END

## Output:

![WhatsApp Image 2025-10-27 at 14 17 54_d9f7dc15](https://github.com/user-attachments/assets/89b902c1-ff73-4131-8442-6604cb40aaab)

![WhatsApp Image 2025-10-27 at 14 18 10_4b5cc923](https://github.com/user-attachments/assets/007a7acb-a7b7-480f-a6a2-593dde3b01d3)

![WhatsApp Image 2025-10-27 at 14 18 21_44a67fdc](https://github.com/user-attachments/assets/1c609a72-74eb-4ffe-a258-72cea1e5055e)

## For Multiplication:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Multiply A and B.
4.	Store the lower byte of the result in memory location 40H.
5.	Store the higher byte of the result in memory location 41H.

## Program:

      ORG 0000H
      MOV A,30H
      MOV B,31H
      MUL AB
      MOV 40H,A
      MOV 41H,B
      END

## Output:

![WhatsApp Image 2025-10-27 at 14 31 19_6969de6e](https://github.com/user-attachments/assets/9d0e4911-a5fc-4d35-b444-1110f2c6b1c2)

![WhatsApp Image 2025-10-27 at 14 32 04_c59c4d07](https://github.com/user-attachments/assets/a1b35280-d409-40d3-89f8-7e46354e704c)

![WhatsApp Image 2025-10-27 at 14 31 37_20be246b](https://github.com/user-attachments/assets/216d3cc0-255c-400a-bb7c-bfc4979d116f)

## For Division:
1.	Load the dividend from memory location 30H into register A.
2.	Load the divisor from memory location 31H into register B.
3.	Divide A by B.
4.	Store the quotient in memory location 40H.
5.	Store the remainder in memory location 41H.


## Program:

      ORG 0000H
      MOV A, 30H
      MOV B, 31H
      DIV AB
      MOV 40H, A
      MOV 41H, B
      END

## Output:

![WhatsApp Image 2025-10-27 at 14 51 19_d24b90df](https://github.com/user-attachments/assets/f7fa8d65-ef62-432a-916c-9a3a9df04c64)

![WhatsApp Image 2025-10-27 at 14 51 39_8f46ace5](https://github.com/user-attachments/assets/8a5d5b12-05a7-492f-a9ca-6db6423caab8)

![WhatsApp Image 2025-10-27 at 14 51 52_453390e0](https://github.com/user-attachments/assets/b768795a-3cec-4840-98d1-e8774540ab7b)

## Result:
The 8-bit arithmetic operations using the 8051 microcontroller have been successfully executed and verified using Keil software.

