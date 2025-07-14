

- Accelerate
-  SparseSolve(\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:)

Solves the equation *Subfactor \* X = B* for the matrix of single-precision values *X*.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ Subfactor: SparseOpaqueSubfactor_Float,
    _ B: DenseMatrix_Float,
    _ X: DenseMatrix_Float
)
```

## Parameters 

`Subfactor`  

The *Subfactor* in *Subfactor* *\* X = B* that SparseCreateSubfactor(_:_:) returns.

`B`  

The matrix *B*.

`X`  

The matrix *X*.

## See Also

### Matrix Solve Functions

func SparseSolve(SparseOpaqueSubfactor_Double, DenseMatrix_Double)

Solves the equation *Subfactor \* X = B* in place for the matrix of double-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseMatrix_Float)

Solves the equation *Subfactor \* X = B* in place for the matrix of single-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Double, DenseMatrix_Double, DenseMatrix_Double)

Solves the equation *Subfactor \* X = B* for the matrix of double-precision values *X*.

