

- Accelerate
-  SparseMultiply(\_:\_:\_:\_:) 

Function

# SparseMultiply(\_:\_:\_:\_:)

Performs the multiply operation *Y* *= Subfactor \* X* on a dense matrix of single-precision values and without any internal memory allocations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseMultiply(
    _ Subfactor: SparseOpaqueSubfactor_Float,
    _ X: DenseMatrix_Float,
    _ Y: DenseMatrix_Float,
    _ workspace: UnsafeMutableRawPointer
)
```

## Parameters 

`Subfactor`  

The subfactor to multiply by, which SparseCreateSubfactor(_:_:) returns.

`X`  

The matrix *X*.

`Y`  

The matrix *Y*.

`workspace`  

A workspace of size `workspaceRequiredStatic` `+ nrhs *` `workspaceRequiredPerRHS` where `nrhs` is the number of right-hand-side vectors.

## See Also

### Subfactor and Dense Matrix Multiplication with User-Defined Workspace

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseMatrix_Double, UnsafeMutableRawPointer)

Performs the multiply operation *Y* *= Subfactor \* X*, in place on a dense matrix of double-precision values and without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseMatrix_Float, UnsafeMutableRawPointer)

Performs the multiply operation *Y* *= Subfactor \* X*, in place on a dense matrix of single-precision values and without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseMatrix_Double, DenseMatrix_Double, UnsafeMutableRawPointer)

Performs the multiply operation *Y* *= Subfactor \* X* on a dense matrix of double-precision values and without any internal memory allocations.

