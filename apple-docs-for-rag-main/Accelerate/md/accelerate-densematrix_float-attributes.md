

- Accelerate
- DenseMatrix_Float
-  attributes 

Instance Property

# attributes

The attributes of the matrix, such as whether it’s symmetrical or triangular.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var attributes: SparseAttributes_t
```

## See Also

### Inspecting a Matrix’s Structure and Data

var rowCount: Int32

The number of rows in the matrix.

var columnCount: Int32

The number of columns in the matrix.

var columnStride: Int32

The stride between matrix columns, in elements.

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

var data: UnsafeMutablePointer&lt;Float>

The array of single-precision, floating-point values in column-major order.

