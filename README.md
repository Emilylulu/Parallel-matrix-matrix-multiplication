# Parallel-matrix-matrix-multiplication
## matrix-matrix-multiplication
You need to write a program, matmult_openmp, that will take as input two files, the matrices A and B, and will output their product. A baseline serial program, matmult, is provided to you as C code. The input and output files for the matrices A, B and C, will be a text representation of a matrix. For an m x n matrix, the file will consist of m+1 lines. The first row will give the dimensions of the matrix and the following m lines will correspond to the rows of the matrix, each made up of n space-separated values, representing the values for each entry in the row. You should assume that the values in the input file are written to exactly four decimal points of precision. Your output file should also follow this convention. For example, a 2 x 4 matrix would be stored in a file as:
24
1.2000 2.3000 3.4000 4.5000 5.6000 6.7000 7.8000 8.9000
You may use the print_matrix function in matmult.c to output the matrix.
## program design
Design your programs so that they follow the following steps:
1. A single thread reads the file.
2. Multiple threads are then working together to do the matrix multiplication. 3. At the end, one thread writes the output.
These are just guidelines, and you should think carefully about step 2.
## Output
Your output file MUST be in the same format as the input files and matrix values must output exactly four decimal points of precision using at most ten characters, i.e., use the "%10.4f" printf pattern when outputting values.
