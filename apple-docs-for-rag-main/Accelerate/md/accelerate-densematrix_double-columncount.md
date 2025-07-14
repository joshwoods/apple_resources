

- Accelerate
- DenseMatrix_Double
-  columnCount 

Instance Property

# columnCount

The number of columns in the matrix.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var columnCount: Int32
```

## See Also

### Inspecting a Matrix’s Structure and Data

var rowCount: Int32

The number of rows in the matrix.

var columnStride: Int32

The stride between matrix columns, in elements.

var attributes: SparseAttributes_t

The attributes of the matrix, such as whether it’s symmetrical or triangular.

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

var data: UnsafeMutablePointer&lt;Double>

The array of double-precision, floating-point values in column-major order.

