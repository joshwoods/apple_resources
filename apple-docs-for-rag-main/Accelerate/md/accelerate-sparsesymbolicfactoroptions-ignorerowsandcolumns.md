

- Accelerate
- SparseSymbolicFactorOptions
-  ignoreRowsAndColumns 

Instance Property

# ignoreRowsAndColumns

An array that contains row and column indices to ignore.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var ignoreRowsAndColumns: UnsafeMutablePointer?
```

## Discussion

If this array isn’t `nil`, ignoreRowsAndColumns provides a list of rows and columns to ignore. Terminate ignoreRowsAndColumns with a negative index.

The row and column indices are for the actual matrix, not its block structure, so `0` indicates the first row, not the first `blockSize` rows.

In the symmetric case (Cholesky, *LDLᵀ*), each entry indicates that the system needs to ignore the matching row and column.

In the unsymmetric case (QR, Cholesky *AᵀA*), consider the matrix, `A`, given the value `m`, with one of the following definitions:

- `m = A.structure.rowCount * A.blockSize` if `A` isn’t a transposed matrix

- `m = A.structure.columnCount * A.blockSize` if `A` is a transposed matrix

In this case, an index less than `m` indicates that the system needs to ignore row `m`. An index `i`, greater than `m`, indicates that the system needs to ignore columns `i - m`.

## See Also

### Inspecting Symbolic Factor Options

var control: SparseControl_t

The flags that control the computation.

struct SparseControl_t

Options that control the computation.

var orderMethod: SparseOrder_t

The ordering algorithm.

var order: UnsafeMutablePointer&lt;Int32>?

The user-supplied array for ordering.

struct SparseOrder_t

Options that define which ordering algorithm to use.

var malloc: (Int) -> UnsafeMutableRawPointer?

The function for allocating any necessary storage.

var free: (UnsafeMutableRawPointer?) -> Void

The function for freeing allocated storage.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

The function for reporting parameter errors.

