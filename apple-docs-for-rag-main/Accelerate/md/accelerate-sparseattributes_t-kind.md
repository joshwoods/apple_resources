

- Accelerate
- SparseAttributes_t
-  kind 

Instance Property

# kind

An eumeration that specifies whether the matrix is ordinary, unit-triangular, triangular, or symmetric.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kind: SparseKind_t { get set }
```

## Mentioned in 

Creating a sparse matrix from coordinate format arrays

## See Also

### Instance Properties

var transpose: Bool

A Boolean value that specifies whether to implicitly transpose the matrix.

var triangle: SparseTriangle_t

An enumeration that specifies which triangle unit-triangular, triangular, and symmetric matrices need to use.

struct SparseTriangle_t

A structure that defines which triangle a symmetric matrix stores, or whether a triangular matrix is upper or lower.

struct SparseKind_t

A structure that defines whether the matrix is ordinary, symmetric, or triangular.

