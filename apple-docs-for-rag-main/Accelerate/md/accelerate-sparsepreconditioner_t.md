

- Accelerate
-  SparsePreconditioner_t 

Structure

# SparsePreconditioner_t

Constants that define the preconditioner type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparsePreconditioner_t
```

## Topics

### Constants

var SparsePreconditionerDiagScaling: SparsePreconditioner_t

A diagonal scaling preconditioner.

var SparsePreconditionerDiagonal: SparsePreconditioner_t

A Jacobi preconditioner.

var SparsePreconditionerNone: SparsePreconditioner_t

No preconditioner.

var SparsePreconditionerUser: SparsePreconditioner_t

A user-provided preconditioner.

### Raw Values

init(Int32)

init(rawValue: Int32)

var rawValue: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Preconditioners

func SparseCreatePreconditioner(SparsePreconditioner_t, SparseMatrix_Double) -> SparseOpaquePreconditioner_Double

Creates a preconditioner for the specified matrix of double-precision values.

func SparseCreatePreconditioner(SparsePreconditioner_t, SparseMatrix_Float) -> SparseOpaquePreconditioner_Float

Creates a preconditioner for the specified matrix of single-precision values.

struct SparseOpaquePreconditioner_Double

A structure that represents a double-precision preconditioner.

struct SparseOpaquePreconditioner_Float

A structure that represents a single-precision preconditioner.

