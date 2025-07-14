

- Accelerate
- SparseSymbolicFactorOptions
-  orderMethod 

Instance Property

# orderMethod

The ordering algorithm.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var orderMethod: SparseOrder_t
```

## See Also

### Inspecting Symbolic Factor Options

var control: SparseControl_t

The flags that control the computation.

struct SparseControl_t

Options that control the computation.

var order: UnsafeMutablePointer&lt;Int32>?

The user-supplied array for ordering.

struct SparseOrder_t

Options that define which ordering algorithm to use.

var ignoreRowsAndColumns: UnsafeMutablePointer&lt;Int32>?

An array that contains row and column indices to ignore.

var malloc: (Int) -> UnsafeMutableRawPointer?

The function for allocating any necessary storage.

var free: (UnsafeMutableRawPointer?) -> Void

The function for freeing allocated storage.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

The function for reporting parameter errors.

