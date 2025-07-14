

- Accelerate
-  SparseCreatePreconditioner(\_:\_:) 

Function

# SparseCreatePreconditioner(\_:\_:)

Creates a preconditioner for the specified matrix of double-precision values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseCreatePreconditioner(
    _ type: SparsePreconditioner_t,
    _ A: SparseMatrix_Double
) -> SparseOpaquePreconditioner_Double
```

## Parameters 

`type`  

The type of preconditioner to create.

`A`  

The matrix to construct a preconditioner for.

## Return Value

A SparseOpaquePreconditioner_Double structure. You must free the resource through a call to SparseCleanup(_:) after you finish with the object.

## See Also

### Preconditioners

struct SparsePreconditioner_t

Constants that define the preconditioner type.

func SparseCreatePreconditioner(SparsePreconditioner_t, SparseMatrix_Float) -> SparseOpaquePreconditioner_Float

Creates a preconditioner for the specified matrix of single-precision values.

struct SparseOpaquePreconditioner_Double

A structure that represents a double-precision preconditioner.

struct SparseOpaquePreconditioner_Float

A structure that represents a single-precision preconditioner.

