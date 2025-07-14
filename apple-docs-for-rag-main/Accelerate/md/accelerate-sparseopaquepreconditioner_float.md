

- Accelerate
-  SparseOpaquePreconditioner_Float 

Structure

# SparseOpaquePreconditioner_Float

A structure that represents a single-precision preconditioner.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseOpaquePreconditioner_Float
```

## Topics

### Creating a Preconditioner

init(type: SparsePreconditioner_t, mem: UnsafeMutableRawPointer, apply: (UnsafeMutableRawPointer, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void)

Creates a new single-precision preconditioner.

### Inspecting Preconditioner Properties

var apply: (UnsafeMutableRawPointer, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void

A function that calculates *Y = PX*, where *P* is the preconditioner.

var mem: UnsafeMutableRawPointer

The unaltered memory pointer that passes as the first parameter of the apply function.

var type: SparsePreconditioner_t

The preconditioner type.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Preconditioners

struct SparsePreconditioner_t

Constants that define the preconditioner type.

func SparseCreatePreconditioner(SparsePreconditioner_t, SparseMatrix_Double) -> SparseOpaquePreconditioner_Double

Creates a preconditioner for the specified matrix of double-precision values.

func SparseCreatePreconditioner(SparsePreconditioner_t, SparseMatrix_Float) -> SparseOpaquePreconditioner_Float

Creates a preconditioner for the specified matrix of single-precision values.

struct SparseOpaquePreconditioner_Double

A structure that represents a double-precision preconditioner.

