

- Accelerate
-  SparseGetTranspose(\_:) 

Function

# SparseGetTranspose(\_:)

Returns a transposed copy of the specified single-precision factorization.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseGetTranspose(_ Factor: SparseOpaqueFactorization_Float) -> SparseOpaqueFactorization_Float
```

## Parameters 

`Factor`  

The factorization to transpose.

## Return Value

A matrix factorization of *A\_\_ᵀ*, where the original was of *A*. Because this is a reference-counted factorization, you must free it through a call to SparseCleanup(_:) when you no longer need it.

## See Also

### Factorization Transpose Functions

func SparseGetTranspose(SparseOpaqueFactorization_Double) -> SparseOpaqueFactorization_Double

Returns a transposed copy of the specified double-precision factorization.

