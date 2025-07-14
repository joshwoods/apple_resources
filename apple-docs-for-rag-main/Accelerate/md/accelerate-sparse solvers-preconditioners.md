

- Accelerate
- Sparse Solvers
-  Preconditioners 

API Collection

# Preconditioners

Create preconditioners for iterative solves.

## Overview

In many cases, applying a preconditioner to the coefficient matrix reduces the number of iterations necessary to solve the system. The Sparse Solvers library provides Jacobi and diagonal scaling preconditioners, and the functionality to create user-defined preconditioners.

## Topics

### Preconditioners

struct SparsePreconditioner_t

Constants that define the preconditioner type.

func SparseCreatePreconditioner(SparsePreconditioner_t, SparseMatrix_Double) -> SparseOpaquePreconditioner_Double

Creates a preconditioner for the specified matrix of double-precision values.

func SparseCreatePreconditioner(SparsePreconditioner_t, SparseMatrix_Float) -> SparseOpaquePreconditioner_Float

Creates a preconditioner for the specified matrix of single-precision values.

struct SparseOpaquePreconditioner_Double

A structure that represents a double-precision preconditioner.

struct SparseOpaquePreconditioner_Float

A structure that represents a single-precision preconditioner.

## See Also

### Solving systems with iterative sparse methods

Solving systems using iterative methods

Use iterative methods to solve systems of equations where the coefficient matrix is sparse.

Sparse Iterative Solving Functions (Matrix RHS)

Solve a system with a right-hand-side dense matrix using iterative methods.

Sparse Iterative Solving Functions (Vector RHS)

Solve a system with a right-hand-side dense vector using iterative methods.

Sparse Iterate Functions

Perform a single iteration of the specified iterative method.

Sparse Iterative Methods

Select a suitable iterative method to solve a system.

