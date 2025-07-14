

- Accelerate
-  SparseOpaqueFactorization_Float 

Structure

# SparseOpaqueFactorization_Float

A structure that represents the factorization of a matrix of single-precision, floating-point values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseOpaqueFactorization_Float
```

## Overview

Use the SparseCleanup(_:) function to free resources that these objects hold.

An object can be in one of the following states:

| **Something is wrong with symbolic factorization, nothing is valid.** | Indication: symbolicFactorization.status `symbolicFactorization.status `>= 0 &&` status `numericFactorization `== NULL`  You can use symbolic factorization for future calls. |
| **Symbolic factorization is good, factor allocation and initialization are correct, but numeric factorization fails.**  For example, the system attempts a Cholesky factorization of an indefinite matrix. | Indication: symbolicFactorization.status `>= 0 &&` status `numericFactorization `not NULL`  You may pass this object to SparseRefactor(_:_:) with a modified matrix. |
| **Symbolic and numeric factorizations are both good.** | Indication: status `>= 0` |

## Topics

### Creating an Opaque Factorization

init()

Creates a new opaque factorization.

init(status: SparseStatus_t, attributes: SparseAttributes_t, symbolicFactorization: SparseOpaqueSymbolicFactorization, userFactorStorage: Bool, numericFactorization: UnsafeMutableRawPointer?, solveWorkspaceRequiredStatic: Int, solveWorkspaceRequiredPerRHS: Int)

Creates a new opaque factorization with the specified parameters.

### Instance Properties

var attributes: SparseAttributes_t

The attributes of a factorization object.

var numericFactorization: UnsafeMutableRawPointer?

The pointer to a private internal representation of a numeric factor.

var solveWorkspaceRequiredPerRHS: Int

The required size of the per-right-hand-side workspace for a call to a sparse solve function.

var solveWorkspaceRequiredStatic: Int

The required size of the static workspace for a call to a sparse solve function.

var status: SparseStatus_t

The status of the factorization object.

var symbolicFactorization: SparseOpaqueSymbolicFactorization

The symbolic factorization that this numeric factorization depends on.

var userFactorStorage: Bool

A Boolean value that indicates whether user-provided storage backs this object.

## See Also

### Solving systems with direct sparse methods

Solving systems using direct methods

Use direct methods to solve systems of equations where the coefficient matrix is sparse.

struct SparseOpaqueFactorization_Double

A structure that represents the factorization of a matrix of double-precision, floating-point values.

Sparse Matrix Factor Functions

Compute the factorization of a matrix.

Sparse Direct Solving Functions (Matrix RHS)

Solve a system with a right-hand-side dense matrix using a factored sparse coefficient matrix.

Sparse Direct Solving Functions (Vector RHS)

Solve a system with a right-hand-side dense vector using a factored sparse coefficient matrix.

Sparse Symbolic Factorization Functions

Calculate the symbolic factorization of a matrix, and solve systems using precalculated symbolic factorizations.

Sparse Refactor Functions

Recompute a factorization using the numerical data from a matrix.

Subfactor Functions

Extract and work with subfactors.

