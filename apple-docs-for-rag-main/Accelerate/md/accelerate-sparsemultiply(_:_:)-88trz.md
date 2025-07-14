

- Accelerate
-  SparseMultiply(\_:\_:) 

Function

# SparseMultiply(\_:\_:)

Performs the multiply operation *Y* *= Subfactor \* X,* \_\_in place on a dense matrix of double-precision values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseMultiply(
    _ Subfactor: SparseOpaqueSubfactor_Double,
    _ XY: DenseMatrix_Double
)
```

## Parameters 

`Subfactor`  

The subfactor to multiply by, which SparseCreateSubfactor(_:_:) returns.

`XY`  

On input, the matrix *X*. On return, the matrix *Y* overwrites it.

## See Also

### Subfactor and Dense Matrix Multiplication

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseMatrix_Float)

Performs the multiply operation *Y*\_ \_*= Subfactor \* X*, in place on a dense matrix of single-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseMatrix_Double, DenseMatrix_Double)

Performs the multiply operation *Y* *= Subfactor \* X* on a dense matrix of double-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseMatrix_Float, DenseMatrix_Float)

Performs the multiply operation *Y* *= Subfactor \* X* on a dense matrix of single-precision values.

