

- Accelerate
- SparseAttributes_t
-  transpose 

Instance Property

# transpose

A Boolean value that specifies whether to implicitly transpose the matrix.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var transpose: Bool { get set }
```

## Discussion

If true, the system implicitly transposes the matrix when it uses it in any functions.

## See Also

### Instance Properties

var triangle: SparseTriangle_t

An enumeration that specifies which triangle unit-triangular, triangular, and symmetric matrices need to use.

struct SparseTriangle_t

A structure that defines which triangle a symmetric matrix stores, or whether a triangular matrix is upper or lower.

var kind: SparseKind_t

An eumeration that specifies whether the matrix is ordinary, unit-triangular, triangular, or symmetric.

struct SparseKind_t

A structure that defines whether the matrix is ordinary, symmetric, or triangular.

