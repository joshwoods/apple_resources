

- Accelerate
- SparseMatrixStructure
-  rowCount 

Instance Property

# rowCount

The number of rows in the matrix.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rowCount: Int32
```

## See Also

### Inspecting the properties of a sparse matrix description

var attributes: SparseAttributes_t

The attributes of the matrix, such as whether it’s symmetrical or triangular.

var blockSize: UInt8

The block size of the matrix.

var columnCount: Int32

The number of columns in the matrix.

var columnStarts: UnsafeMutablePointer&lt;Int>

The starting index for each column in the row indices array.

var rowIndices: UnsafeMutablePointer&lt;Int32>

The row indices of the matrix.

