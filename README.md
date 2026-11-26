for simple test case, answers are stored in 0x000003b4, 0x000003b8, and 0x000003bc. It should be equal to 1, 3, and 5 respectively. 

for 32 x 32 test case, answers are stored in 0x13d0, 0x13d4, so on. It should be 0x20, 0x40, 0x60 and so on respectively.

for part 2, answers are stored in 0x1404 and on. Answers are same as part 1 32x32 test case.

to change matrix dimension, find "li a3, xx" and set that to the desired dimension. 
then find 
"la a0, matrix
li a1, xx          // number of rows
li a2, xx          // number of columns
la a4, sum" and change the values there
then find the memory allocation
".data

matrix: .space 4096
sum:    .space 128" and change the values there
