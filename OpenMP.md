# Part B - OpenMP Matrix Multiplication

## 1. OpenMPI Setup

OpenMPI and OpenSSH were configured on the required Ubuntu systems for distributed matrix multiplication.

## 2. MPI Program

The matrix multiplication program was implemented using MPI to distribute the computation across multiple processes.

## 3. Working and Output

The OpenMP matrix multiplication program was compiled and executed successfully using 8 threads.

The program performed multiplication of two 4000 × 4000 matrices and verified the result successfully.

<img width="762" height="294" alt="openmp" src="https://github.com/user-attachments/assets/553569cd-33ad-4bb8-90e2-89ffd1049572" />

## 4. Result

The OpenMP implementation completed successfully with an execution time of **40.545825 seconds**.

The verification value was **C[0][0] = 4000.00**, confirming the correctness of the matrix multiplication.
