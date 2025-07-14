

- Accelerate
-  SparseGMRES(\_:) 

Function

# SparseGMRES(\_:)

Returns a generalized minimal residual (GMRES) method with specified options.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseGMRES(_ options: SparseGMRESOptions) -> SparseIterativeMethod
```

## Parameters 

`options`  

The options to use when creating the GMRES method, such as the maximum number of iterations to perform.

## Return Value

A SparseIterativeMethod structure that represents a generalized minimal residual (GMRES) method.

## Discussion

Use GMRES to solve *Ax = b* when *A* is symmetric indefinite or unsymmetric.

For symmetric positive-definite systems, use SparseConjugateGradient(_:). For rectangular or singular systems, use SparseLSMR(_:).

## See Also

### Sparse Iterative Methods for Symmetric Indefinite and Unsymmetric Coefficient Matrices

func SparseGMRES() -> SparseIterativeMethod

Returns a generalized minimal residual (GMRES) method.

struct SparseGMRESOptions

Options for creating a generalized minimal residual (GMRES) method.

