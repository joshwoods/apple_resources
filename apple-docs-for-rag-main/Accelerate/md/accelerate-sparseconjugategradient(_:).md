

- Accelerate
-  SparseConjugateGradient(\_:) 

Function

# SparseConjugateGradient(\_:)

Returns a conjugate gradient (CG) method with specified options.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseConjugateGradient(_ options: SparseCGOptions) -> SparseIterativeMethod
```

## Parameters 

`options`  

The options to use when creating the conjugate gradient method, such as the maximum number of iterations to perform.

## Return Value

A SparseIterativeMethod structure that represents a default conjugate gradient method.

## Discussion

Use CG to solve *Ax = b* when *A* is symmetric positive-definite. The method may break down or fail to converge if *A* isn’t positive-definite.

For square, full-rank, unsymmetric or indefinite equations, use SparseGMRES(_:). For rectangular or singular systems, use SparseLSMR(_:).

## See Also

### Sparse Iterative Methods for Symmetric Positive-Definite Coefficient Matrices

func SparseConjugateGradient() -> SparseIterativeMethod

Returns a conjugate gradient (CG) method.

struct SparseCGOptions

Options for creating a conjugate gradient (CG) method.

