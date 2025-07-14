

- Accelerate
-  SparseMultiply(\_:\_:\_:) 

Function

# SparseMultiply(\_:\_:\_:)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseMultiply(
    _ Subfactor: SparseOpaqueSubfactor_Double,
    _ X: DenseVector_Double,
    _ Y: DenseVector_Double
)
```

## Parameters 

`Subfactor`  

The subfactor to multiply by, which SparseCreateSubfactor(_:_:) returns.

`X`  

The vector *X*.

`Y`  

The vector *Y*.

## See Also

### Subfactor and Dense Vector Multiplication

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseVector_Double)

Performs the multiply operation *Y = Subfactor \* X*, in place on a vector of double-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float)

Performs the multiply operation *Y = Subfactor \* X*, in place on a vector of single-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *Y = Subfactor \** *X* on a vector of single-precision values.

