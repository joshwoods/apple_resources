

- Accelerate
-  SparseSolve(\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:)

Solves the equation *Subfactor \* X = B* for the vector of double-precision values *X*, in place and without any internal memory allocations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ Subfactor: SparseOpaqueSubfactor_Double,
    _ XB: DenseVector_Double,
    _ workspace: UnsafeMutableRawPointer
)
```

## Parameters 

`Subfactor`  

The *Subfactor* in *Subfactor* *\* X = B* that SparseCreateSubfactor(_:_:) returns.

`XB`  

On input, the vector *B*. On return, the vector *X* overwrites it.

`workspace`  

A workspace of size `workspaceRequiredStatic` `+` `workspaceRequiredPerRHS`.

## See Also

### Vector Solve Functions with User-Defined Workspace

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of single-precision values *X*, in place and without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Double, DenseVector_Double, DenseVector_Double, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of double-precision values *X*, without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of single-precision values *X*, without any internal memory allocations.

