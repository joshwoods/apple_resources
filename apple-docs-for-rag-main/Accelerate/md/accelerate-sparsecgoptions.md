

- Accelerate
-  SparseCGOptions 

Structure

# SparseCGOptions

Options for creating a conjugate gradient (CG) method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseCGOptions
```

## Overview

Use CG to solve *Ax = b* when *A* is symmetric positive-definite. The method may break down or fail to converge if *A* isn’t positive-definite.

For square, full-rank, unsymmetric or indefinite equations, use SparseGMRES(_:). For rectangular or singular systems, use SparseLSMR(_:).

## Topics

### Initializers

init()

Returns a new CG options structure.

init(reportError: ((UnsafePointer&lt;CChar>) -> Void)?, maxIterations: Int32, atol: Double, rtol: Double, reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?)

Returns a new CG options structure using the specified parameters.

### Inspecting CG Options

var atol: Double

The absolute convergence tolerance.

var maxIterations: Int32

The maximum number of iterations to perform.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

var rtol: Double

The relative convergence tolerance.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Sparse Iterative Methods for Symmetric Positive-Definite Coefficient Matrices

func SparseConjugateGradient() -> SparseIterativeMethod

Returns a conjugate gradient (CG) method.

func SparseConjugateGradient(SparseCGOptions) -> SparseIterativeMethod

Returns a conjugate gradient (CG) method with specified options.

