By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**

![image](https://github.com/Mamthag17/task3.md/assets/161347200/284559e6-896f-4fb7-96d0-b0421f8eb964)
**Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c& 

![image](https://github.com/Mamthag17/task3.md/assets/161347200/6daf2d7c-40e4-4ce2-b64d-3043dc532cfc)
Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c 

![image](https://github.com/Mamthag17/task3.md/assets/161347200/4daf6f73-6e6e-4fe7-ba05-1a054509742e)
Step 5: Check the output by using the command

./a.out

![image](https://github.com/Mamthag17/task3.md/assets/161347200/5f55c825-0bf1-49a2-828f-c963f2c516b9)
The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c

![image](https://github.com/Mamthag17/task3.md/assets/161347200/1e2aa54c-3e5c-4a48-8385-0b08e8400db6)
Step 2: Compile the code in riscv using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![image](https://github.com/Mamthag17/task3.md/assets/161347200/37d81bce-09e1-4a35-b554-db206d05c8b7)
Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command ls -ltr sum1ton.c

![image](https://github.com/Mamthag17/task3.md/assets/161347200/9f8f23aa-2947-4376-9513-3e3fd90be00f)

![image](https://github.com/Mamthag17/task3.md/assets/161347200/bbd212d9-ae10-4b89-a48c-bc5e1a3d0d68)
Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution

![image](https://github.com/Mamthag17/task3.md/assets/161347200/57e6dd0a-8378-41d7-9f93-d8ccaa640b60)

![image](https://github.com/Mamthag17/task3.md/assets/161347200/b2de93cf-e043-4383-abfe-b3f378cae952)
Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![image](https://github.com/Mamthag17/task3.md/assets/161347200/ac0253e5-812e-4be4-98c0-e50769bb4383)

![image](https://github.com/Mamthag17/task3.md/assets/161347200/e1a44d45-75c4-4569-af07-04561c3d2582)
