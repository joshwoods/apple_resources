

- Accelerate
-  SparseGMRESOptions 

Structure

# SparseGMRESOptions

Options for creating a generalized minimal residual (GMRES) method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseGMRESOptions
```

## Overview

Use GMRES to solve *Ax = b* when *A* is symmetric indefinite or unsymmetric.

For symmetric positive-definite systems, use SparseConjugateGradient(_:). For rectangular or singular systems, use SparseLSMR(_:).

## Topics

### Initializers

init()

init(reportError: ((UnsafePointer&lt;CChar>) -> Void)?, variant: SparseGMRESVariant_t, nvec: Int32, maxIterations: Int32, atol: Double, rtol: Double, reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?)

Returns a new GMRES options structure using the specified parameters.

### Inspecting GMRES Options

var atol: Double

The absolute convergence tolerance.

var maxIterations: Int32

The maximum number of iterations to perform.

var nvec: Int32

The number of orthogonal vectors the operation maintains.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

The function to report status.

var rtol: Double

The relative convergence tolerance.

var variant: SparseGMRESVariant_t

The exact variant of GMRES to implement.

struct SparseGMRESVariant_t

Defines the exact variant of GMRES to implement

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Sparse Iterative Methods for Symmetric Indefinite and Unsymmetric Coefficient Matrices

func SparseGMRES() -> SparseIterativeMethod

Returns a generalized minimal residual (GMRES) method.

func SparseGMRES(SparseGMRESOptions) -> SparseIterativeMethod

Returns a generalized minimal residual (GMRES) method with specified options.

