

- Accelerate
-  SparseMultiply(\_:\_:\_:) 

Function

# SparseMultiply(\_:\_:\_:)

Performs the multiply operation *Y = Subfactor \* X* on a vector of single-precision values *X*, in place and without any internal memory allocations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseMultiply(
    _ Subfactor: SparseOpaqueSubfactor_Float,
    _ XY: DenseVector_Float,
    _ workspace: UnsafeMutableRawPointer
)
```

## Parameters 

`Subfactor`  

The subfactor to multiply by, which SparseCreateSubfactor(_:_:) returns.

`XY`  

On input, the vector *Y*. On return, the vector *Y* overwrites it.

`workspace`  

A workspace of size `workspaceRequiredStatic` `+` `workspaceRequiredPerRHS`.

## See Also

### Subfactor and Dense Vector Multiplication with User-Defined Workspace

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseVector_Double, UnsafeMutableRawPointer)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values *X*, in place and without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseVector_Double, DenseVector_Double, UnsafeMutableRawPointer)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values *X*, without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float, UnsafeMutableRawPointer)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values *X*, without any internal memory allocations.

