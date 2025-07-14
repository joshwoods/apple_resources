

- Accelerate
-  SparseTriangle_t 

Structure

# SparseTriangle_t

A structure that defines which triangle a symmetric matrix stores, or whether a triangular matrix is upper or lower.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseTriangle_t
```

## Topics

### Constants

var SparseLowerTriangle: SparseTriangle_t

A constant that specifies the lower triangle.

var SparseUpperTriangle: SparseTriangle_t

A constant that specifies the upper triangle.

### Raw Values

init(UInt8)

init(rawValue: UInt8)

var rawValue: UInt8

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

var kind: SparseKind_t

An eumeration that specifies whether the matrix is ordinary, unit-triangular, triangular, or symmetric.

struct SparseKind_t

A structure that defines whether the matrix is ordinary, symmetric, or triangular.

