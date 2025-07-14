

- Accelerate
- SparseSymbolicFactorOptions
-  reportError 

Instance Property

# reportError

The function for reporting parameter errors.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var reportError: ((UnsafePointer) -> Void)?
```

## Mentioned in 

Solving systems using direct methods

## Discussion

If this value is `nil`, the system reports errors using os_log_error and then `__builtin_trap()`.

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

var ignoreRowsAndColumns: UnsafeMutablePointer&lt;Int32>?

An array that contains row and column indices to ignore.

var malloc: (Int) -> UnsafeMutableRawPointer?

The function for allocating any necessary storage.

var free: (UnsafeMutableRawPointer?) -> Void

The function for freeing allocated storage.

