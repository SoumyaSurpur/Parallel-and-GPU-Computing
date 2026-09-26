# Parallel-and-GPU-Computing

## Experiments

### 1. Sequential Matrix Multiplication

A baseline matrix multiplication implementation using sequential CPU execution.

In this implementation, the complete matrix multiplication is performed by a single CPU process using three nested loops. Two 4000 × 4000 matrices are initialized with values of 1.0, and the result matrix is computed sequentially.

The implementation is used as the baseline for comparing the performance of parallel approaches.

**Matrix Size:** 4000 × 4000  
**Execution Model:** Single CPU Process  
**Verification:** C[0][0] = 4000.00

[View Sequential Experiment](https://github.com/SoumyaSurpur/Parallel-and-GPU-Computing/blob/main/Sequential.md)


### 2. OpenMP Matrix Multiplication

A shared-memory parallel implementation using OpenMP and multiple CPU threads.

The matrix multiplication is parallelized using OpenMP, allowing multiple CPU threads to perform different parts of the computation concurrently. In this experiment, 8 OpenMP threads are used to process the 4000 × 4000 matrix.

The OpenMP implementation is compared with the sequential baseline to observe the effect of CPU-based parallel execution.

**Matrix Size:** 4000 × 4000  
**Execution Model:** Shared-Memory Parallelism  
**OpenMP Threads:** 8  
**Verification:** C[0][0] = 4000.00

[View OpenMP Experiment](https://github.com/SoumyaSurpur/Parallel-and-GPU-Computing/blob/main/OpenMP.md)

### 3. MPI Matrix Multiplication

A distributed-memory implementation using MPI across multiple processes and virtual machines.

[View MPI Experiment](./MPI.md)

### 4. CUDA Matrix Multiplication

A GPU-based implementation using CUDA for parallel matrix multiplication.

[View CUDA Experiment](./CUDA.md)

## Problem Definition

The matrix multiplication experiment uses:

- Matrix A: 4000 × 4000
- Matrix B: 4000 × 4000
- Matrix C: A × B
- Matrix elements: 1.0
- Expected verification: C[0][0] = 4000.00

## Technologies Used

- C
- GCC
- Ubuntu
- WSL2
- OpenMP
- MPI
- CUDA

## Repository Structure

```text
Parallel-and-GPU-Computing/
│
├── README.md
├── Sequential.md
├── OpenMP.md
├── MPI.md
└── CUDA.md

