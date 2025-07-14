

- Accelerate
-  SparseLSMROptions 

Structure

# SparseLSMROptions

Options for creating a least squares minimum residual method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseLSMROptions
```

## Overview

LSMR is a minimal residual (MINRES) method for solving least squares. Use LSMR to solve equations of the form *Ax = b* where an exact solution doesn’t exist. The returned solution minimizes ‖ *b-Ax* ‖₂.

Although LSMR is equivalent to applying MINRES to the normal equations *A\_\_ᵀ\_\_Ax = A\_\_ᵀ\_\_b* in exact arithmetic, it has superior numerical behavior and is the preferred method. Due to the implicit squaring of the condition of *A* in the normal equations, LSMR may struggle to converge in single precision. Use double-precision arithmetic where possible.

For symmetric positive-definite systems, use SparseConjugateGradient(_:). For square, full-rank unsymmetric or indefinite equations, use SparseGMRES(_:).

## Topics

### Initializers

init()

Returns a new LSMR options structure.

init(reportError: ((UnsafePointer&lt;CChar>) -> Void)?, lambda: Double, nvec: Int32, convergenceTest: SparseLSMRConvergenceTest_t, atol: Double, rtol: Double, btol: Double, conditionLimit: Double, maxIterations: Int32, reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?)

Returns a new LSMR options structure using the specified parameters.

### Inspecting LSMR Options

var atol: Double

The absolute tolerance (default test) or *A* tolerance (Fong-Saunders test).

var btol: Double

The *B* tolerance (Fong-Saunders test only).

var conditionLimit: Double

The condition number limit (Fong-Saunders test only).

var convergenceTest: SparseLSMRConvergenceTest_t

The convergence test to use for iterative solve methods.

struct SparseLSMRConvergenceTest_t

Constants that specify the type of convergence test.

var lambda: Double

The damping parameter lambda for regularized least squares.

var maxIterations: Int32

The maximum number of iterations.

var nvec: Int32

The number of vectors to use for local reorthogonalization.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

An optional error-reporting routine.

var reportStatus: ((UnsafePointer&lt;CChar>) -> Void)?

An optional status-reporting routine.

var rtol: Double

The relative convergence tolerance (default test only).

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Sparse Iterative Methods for Overdetermined and Underdetermined Systems

func SparseLSMR() -> SparseIterativeMethod

Returns a default least squares minimum residual (LSMR) method.

func SparseLSMR(SparseLSMROptions) -> SparseIterativeMethod

Returns a least squares minimum residual method with specified options.

