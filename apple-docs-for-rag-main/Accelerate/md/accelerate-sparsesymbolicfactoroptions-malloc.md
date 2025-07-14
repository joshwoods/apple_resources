

- Accelerate
- SparseSymbolicFactorOptions
-  malloc 

Instance Property

# malloc

The function for allocating any necessary storage.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var malloc: (Int) -> UnsafeMutableRawPointer?
```

## Parameters 

`size`  

The size of space to allocate in bytes.

## Return Value

A pointer to newly allocated memory, or `nil` if allocation fails.

## Discussion

The system frees memory through the free callback. If this function pointer is `nil`, the system uses `malloc()`.

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

var free: (UnsafeMutableRawPointer?) -> Void

The function for freeing allocated storage.

var reportError: ((UnsafePointer&lt;CChar>) -> Void)?

The function for reporting parameter errors.

