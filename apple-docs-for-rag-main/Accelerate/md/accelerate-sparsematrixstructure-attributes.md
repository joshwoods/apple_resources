

- Accelerate
- SparseMatrixStructure
-  attributes 

Instance Property

# attributes

The attributes of the matrix, such as whether it’s symmetrical or triangular.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var attributes: SparseAttributes_t
```

## Mentioned in 

Creating sparse matrices

## See Also

### Inspecting the properties of a sparse matrix description

var blockSize: UInt8

The block size of the matrix.

var columnCount: Int32

The number of columns in the matrix.

var columnStarts: UnsafeMutablePointer&lt;Int>

The starting index for each column in the row indices array.

var rowCount: Int32

The number of rows in the matrix.

var rowIndices: UnsafeMutablePointer&lt;Int32>

The row indices of the matrix.

