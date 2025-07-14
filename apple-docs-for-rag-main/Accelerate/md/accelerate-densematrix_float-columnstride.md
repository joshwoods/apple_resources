

- Accelerate
- DenseMatrix_Float
-  columnStride 

Instance Property

# columnStride

The stride between matrix columns, in elements.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var columnStride: Int32
```

## See Also

### Inspecting a Matrix’s Structure and Data

var rowCount: Int32

The number of rows in the matrix.

var columnCount: Int32

The number of columns in the matrix.

var attributes: SparseAttributes_t

The attributes of the matrix, such as whether it’s symmetrical or triangular.

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

var data: UnsafeMutablePointer&lt;Float>

The array of single-precision, floating-point values in column-major order.

