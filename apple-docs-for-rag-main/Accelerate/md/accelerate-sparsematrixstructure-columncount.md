

- Accelerate
- SparseMatrixStructure
-  columnCount 

Instance Property

# columnCount

The number of columns in the matrix.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var columnCount: Int32
```

## See Also

### Inspecting the properties of a sparse matrix description

var attributes: SparseAttributes_t

The attributes of the matrix, such as whether it’s symmetrical or triangular.

var blockSize: UInt8

The block size of the matrix.

var columnStarts: UnsafeMutablePointer&lt;Int>

The starting index for each column in the row indices array.

var rowCount: Int32

The number of rows in the matrix.

var rowIndices: UnsafeMutablePointer&lt;Int32>

The row indices of the matrix.

