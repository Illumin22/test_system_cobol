IDENTIFICATION DIVISION.
       PROGRAM-ID. HELLO.

           DATA DIVISION.
           WORKING-STORAGE SECTION.
           01 Choice1 PIC X(1).
           01 UserName1 PIC A(5).
           01 Password1 PIC A(5).
           01 Name1 PIC A(22) value "Mark Julius Hernandez".
           01 CODE1 PIC X(6) value "123456".
           PROCEDURE DIVISION.
           
           DISPLAY "1. Existing Card".
           DISPLAY "2. ADMIN LOG IN".
           DISPLAY "3. EXIT".
           DISPLAY "Enter Your Choice : ".
           ACCEPT Choice1.
           IF Choice1 = 1 THEN 
               DISPLAY "***BDO ATM MACHINE***". 
               DISPLAY "ENTER NAME :               " .
               ACCEPT Name1.
               DISPLAY "ENTER PIN NUMBER :         ".
               ACCEPT CODE1.
               IF Name1 = "Mark Julius Hernandez" and CODE1 = "123456" 
                   then DISPLAY "WELOME USER!"
                   else DISPLAY "Invalid Credentials"
               
                end-if.
            IF Choice1 = 2 then 
               DISPLAY "Admin log in".
               DISPLAY "USERNAME : " UserName1.
                ACCEPT UserName1.
               DISPLAY "PASSWORD :  "Password1.
                ACCEPT Password1.
               IF UserName1 is equal to 123 and  Password1 is equal to
               1234 then DISPLAY "WELCOME ADMIN."

               ELSE 
               DISPLAY "Error! Invalid Credentials!".
            IF Choice1 = 3 then 
               DISPLAY "THANK YOU! COME AGAIN".
           STOP RUN.
