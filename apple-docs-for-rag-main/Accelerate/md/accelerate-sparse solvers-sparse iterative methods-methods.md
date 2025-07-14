

- Accelerate
- Sparse Solvers
-  Sparse Iterative Methods 

API Collection

# Sparse Iterative Methods

Select a suitable iterative method to solve a system.

## Overview

Sparse Iterative methods solve *Ax = b* through an iterative process that only requires multiplication by *A* or *A\_\_ᵀ*. However, if *A* is numerically difficult, the iterative process may fail to converge to a solution. Even for problems where the process converges, it may do so slowly. You can fix both of these issues through the application of a problem-specific preconditioner that approximates the inverse of *A*.

## Topics

### Sparse Iterative Methods for Symmetric Positive-Definite Coefficient Matrices

func SparseConjugateGradient() -> SparseIterativeMethod

Returns a conjugate gradient (CG) method.

func SparseConjugateGradient(SparseCGOptions) -> SparseIterativeMethod

Returns a conjugate gradient (CG) method with specified options.

struct SparseCGOptions

Options for creating a conjugate gradient (CG) method.

### Sparse Iterative Methods for Symmetric Indefinite and Unsymmetric Coefficient Matrices

func SparseGMRES() -> SparseIterativeMethod

Returns a generalized minimal residual (GMRES) method.

func SparseGMRES(SparseGMRESOptions) -> SparseIterativeMethod

Returns a generalized minimal residual (GMRES) method with specified options.

struct SparseGMRESOptions

Options for creating a generalized minimal residual (GMRES) method.

### Sparse Iterative Methods for Overdetermined and Underdetermined Systems

func SparseLSMR() -> SparseIterativeMethod

Returns a default least squares minimum residual (LSMR) method.

func SparseLSMR(SparseLSMROptions) -> SparseIterativeMethod

Returns a least squares minimum residual method with specified options.

struct SparseLSMROptions

Options for creating a least squares minimum residual method.

### Iterative Method Structure

struct SparseIterativeMethod

The base type for all iterative methods.

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

Preconditioners

Create preconditioners for iterative solves.

