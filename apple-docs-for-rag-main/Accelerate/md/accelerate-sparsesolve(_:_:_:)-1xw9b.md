

- Accelerate
-  SparseSolve(\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:)

Solves the equation *Subfactor \* X = B* for the vector of single-precision values *X*, in place and without any internal memory allocations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func SparseSolve(
    _ Subfactor: SparseOpaqueSubfactor_Float,
    _ XB: DenseVector_Float,
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

func SparseSolve(SparseOpaqueSubfactor_Double, DenseVector_Double, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of double-precision values *X*, in place and without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Double, DenseVector_Double, DenseVector_Double, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of double-precision values *X*, without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of single-precision values *X*, without any internal memory allocations.

