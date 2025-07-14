

- Accelerate
-  SparseSolve(\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:)

Solves the equation *Subfactor \* X = B* in place for the vector of double-precision values *X*.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ Subfactor: SparseOpaqueSubfactor_Double,
    _ B: DenseVector_Double,
    _ X: DenseVector_Double
)
```

## Parameters 

`Subfactor`  

The *Subfactor* in *Subfactor* *\* X = B* that SparseCreateSubfactor(_:_:) returns.

`B`  

The vector *B*.

`X`  

The vector *X*.

## See Also

### Vector Solve Functions

func SparseSolve(SparseOpaqueSubfactor_Double, DenseVector_Double)

Solves the equation *Subfactor \* X = B* in place for the vector of double-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float)

Solves the equation *Subfactor \* X = B* in place for the vector of single-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float)

Solves the equation *Subfactor \* X = B* in place for the vector of single-precision values *X*.

