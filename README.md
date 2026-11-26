to find where sum is stored, look at the value in a4, that value is the starting address of sum.
to find where the matrix is stored, place an ebreak after "la t4, matrix" and look at the value in t4, that is the starting address of the matrix.

to change matrix dimension, find "li a3, xx" and set that to the desired dimension,

then find 
"la a0, matrix
li a1, xx          // number of rows
li a2, xx          // number of columns
la a4, sum" and change the values there

then find the memory allocation
".data
matrix: .space 4096
sum:    .space 128" and change the values there
