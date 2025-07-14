

- Accelerate
-  SparseLSMR(\_:) 

Function

# SparseLSMR(\_:)

Returns a least squares minimum residual method with specified options.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseLSMR(_ options: SparseLSMROptions) -> SparseIterativeMethod
```

## Parameters 

`options`  

The LSMR options to use when creating the LSMR method.

## Return Value

A SparseIterativeMethod structure that represents a default LSMR method.

## Discussion

LSMR is a minimal residual (MINRES) method for solving least squares. Use LSMR to solve equations of the form *Ax = b* where an exact solution doesn’t exist. The returned solution minimizes ‖ *b-Ax* ‖₂.

Although LSMR is equivalent to applying MINRES to the normal equations *AᵀAx = Aᵀb* in exact arithmetic, it has superior numerical behavior and is the preferred method. Due to the implicit squaring of the condition of *A* in the normal equations, LSMR may struggle to converge in single precision. Use double-precision arithmetic where possible.

For symmetric positive-definite systems, use SparseConjugateGradient(_:). For square, full-rank unsymmetric or indefinite equations, use SparseGMRES(_:).

## See Also

### Sparse Iterative Methods for Overdetermined and Underdetermined Systems

func SparseLSMR() -> SparseIterativeMethod

Returns a default least squares minimum residual (LSMR) method.

struct SparseLSMROptions

Options for creating a least squares minimum residual method.

