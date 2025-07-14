

- Accelerate
-  SparseMultiply(\_:\_:) 

Function

# SparseMultiply(\_:\_:)

Performs the multiply operation *Y = Subfactor \* X*, in place on a vector of double-precision values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseMultiply(
    _ Subfactor: SparseOpaqueSubfactor_Double,
    _ XY: DenseVector_Double
)
```

## Parameters 

`Subfactor`  

The subfactor to multiply by, which SparseCreateSubfactor(_:_:) returns.

`XY`  

On input, the vector *X*. On return, the vector *Y* overwrites it.

## See Also

### Subfactor and Dense Vector Multiplication

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float)

Performs the multiply operation *Y = Subfactor \* X*, in place on a vector of single-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseVector_Double, DenseVector_Double)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *Y = Subfactor \** *X* on a vector of single-precision values.

