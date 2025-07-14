

- Accelerate
- SparseSymbolicFactorOptions
-  init(control:orderMethod:order:ignoreRowsAndColumns:malloc:free:reportError:) 

Initializer

# init(control:orderMethod:order:ignoreRowsAndColumns:malloc:free:reportError:)

Creates a new structure that contains options that affect the symbolic stage of a sparse factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    control: SparseControl_t,
    orderMethod: SparseOrder_t,
    order: UnsafeMutablePointer?,
    ignoreRowsAndColumns: UnsafeMutablePointer?,
    malloc: (Int) -> UnsafeMutableRawPointer?,
    free: (UnsafeMutableRawPointer?) -> Void,
    reportError: ((UnsafePointer) -> Void)?
)
```

## Parameters 

`control`  

The flags that control the computation.

`orderMethod`  

The ordering algorithm.

`order`  

The user-supplied array for ordering.

`ignoreRowsAndColumns`  

An array that contains row and column indices to ignore.

`malloc`  

The function for allocating any necessary storage.

`free`  

The function for freeing allocated storage.

`reportError`  

The function for reporting parameter errors.

