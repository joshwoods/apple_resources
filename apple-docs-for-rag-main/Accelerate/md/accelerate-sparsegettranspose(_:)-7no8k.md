

- Accelerate
-  SparseGetTranspose(\_:) 

Function

# SparseGetTranspose(\_:)

Returns a transposed copy of the specified matrix of single-precision, floating-point values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseGetTranspose(_ Matrix: SparseMatrix_Float) -> SparseMatrix_Float
```

## Parameters 

`Matrix`  

The matrix to transpose.

## Return Value

A SparseMatrix_Float structure that represents the transposed matrix.

## Discussion

Use this function to return a new SparseMatrix_Double structure that shares underlying storage with the specified matrix, but with its transpose attribute as `true`. The system doesn’t reference-count the underlying storage, so you must ensure it doesn’t destroy the original matrix before you finish with the matrix that this routine returns.

## See Also

### Matrix Transpose Functions

func SparseGetTranspose(SparseMatrix_Double) -> SparseMatrix_Double

Returns a transposed copy of the specified matrix of double-precision, floating-point values.

