

- Accelerate
-  SparseKind_t 

Structure

# SparseKind_t

A structure that defines whether the matrix is ordinary, symmetric, or triangular.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseKind_t
```

## Topics

### Constants

var SparseOrdinary: SparseKind_t

An unsymmetric sparse matrix without special structure.

var SparseSymmetric: SparseKind_t

A symmetric sparse matrix.

var SparseTriangular: SparseKind_t

A triangular sparse matrix with a nonunit diagonal.

var SparseUnitTriangular: SparseKind_t

A triangular sparse matrix with a unit diagonal.

### Raw Values

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Instance Properties

var transpose: Bool

A Boolean value that specifies whether to implicitly transpose the matrix.

var triangle: SparseTriangle_t

An enumeration that specifies which triangle unit-triangular, triangular, and symmetric matrices need to use.

struct SparseTriangle_t

A structure that defines which triangle a symmetric matrix stores, or whether a triangular matrix is upper or lower.

var kind: SparseKind_t

An eumeration that specifies whether the matrix is ordinary, unit-triangular, triangular, or symmetric.

