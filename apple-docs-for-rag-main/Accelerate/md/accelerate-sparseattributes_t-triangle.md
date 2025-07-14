

- Accelerate
- SparseAttributes_t
-  triangle 

Instance Property

# triangle

An enumeration that specifies which triangle unit-triangular, triangular, and symmetric matrices need to use.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var triangle: SparseTriangle_t { get set }
```

## Discussion

If kind is SparseOrdinary, this operation ignores this propoerty. Otherwise, it indicates which triangle (SparseUpperTriangle or SparseLowerTriangle) represents the matrix.

## See Also

### Instance Properties

var transpose: Bool

A Boolean value that specifies whether to implicitly transpose the matrix.

struct SparseTriangle_t

A structure that defines which triangle a symmetric matrix stores, or whether a triangular matrix is upper or lower.

var kind: SparseKind_t

An eumeration that specifies whether the matrix is ordinary, unit-triangular, triangular, or symmetric.

struct SparseKind_t

A structure that defines whether the matrix is ordinary, symmetric, or triangular.

