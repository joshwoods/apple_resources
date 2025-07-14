

- Accelerate
- SparseMatrixStructure
-  columnStarts 

Instance Property

# columnStarts

The starting index for each column in the row indices array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var columnStarts: UnsafeMutablePointer
```

## Discussion

This array requires an additional, final entry that defines the final column’s length.

## See Also

### Inspecting the properties of a sparse matrix description

var attributes: SparseAttributes_t

The attributes of the matrix, such as whether it’s symmetrical or triangular.

var blockSize: UInt8

The block size of the matrix.

var columnCount: Int32

The number of columns in the matrix.

var rowCount: Int32

The number of rows in the matrix.

var rowIndices: UnsafeMutablePointer&lt;Int32>

The row indices of the matrix.

