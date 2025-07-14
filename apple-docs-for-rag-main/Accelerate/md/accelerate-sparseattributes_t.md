

- Accelerate
-  SparseAttributes_t 

Structure

# SparseAttributes_t

A structure that represents the attributes of a matrix.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseAttributes_t
```

## Mentioned in 

Creating sparse matrices

## Topics

### Creating a New Attributes Structure

init()

Returns a new sparse attributes structure.

### Instance Properties

var transpose: Bool

A Boolean value that specifies whether to implicitly transpose the matrix.

var triangle: SparseTriangle_t

An enumeration that specifies which triangle unit-triangular, triangular, and symmetric matrices need to use.

struct SparseTriangle_t

A structure that defines which triangle a symmetric matrix stores, or whether a triangular matrix is upper or lower.

var kind: SparseKind_t

An eumeration that specifies whether the matrix is ordinary, unit-triangular, triangular, or symmetric.

struct SparseKind_t

A structure that defines whether the matrix is ordinary, symmetric, or triangular.

## Relationships

### Conforms To

- Sendable

## See Also

### Inspecting a Matrix’s Structure and Data

var rowCount: Int32

The number of rows in the matrix.

var columnCount: Int32

The number of columns in the matrix.

var columnStride: Int32

The stride between matrix columns, in elements.

var attributes: SparseAttributes_t

The attributes of the matrix, such as whether it’s symmetrical or triangular.

var data: UnsafeMutablePointer&lt;Double>

The array of double-precision, floating-point values in column-major order.

