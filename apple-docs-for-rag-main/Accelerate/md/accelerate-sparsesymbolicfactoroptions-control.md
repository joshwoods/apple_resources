

- Accelerate
- SparseSymbolicFactorOptions
-  control 

Instance Property

# control

The flags that control the computation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var control: SparseControl_t
```

## See Also

### Inspecting Symbolic Factor Options

struct SparseControl_t

Options that control the computation.

var orderMethod: SparseOrder_t

The ordering algorithm.

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

