

- Accelerate
- BNNSFilterParameters
-  init(flags:n_threads:alloc_memory:free_memory:) 

Initializer

# init(flags:n_threads:alloc_memory:free_memory:)

Returns a new common filter parameters structure.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    flags: UInt32,
    n_threads: Int,
    alloc_memory: BNNSAlloc?,
    free_memory: BNNSFree?
)
```

## Parameters 

`flags`  

A logical OR of zero or more values from BNNS flags.

`n_threads`  

The maximum number of threads that the filter executes. Set to `0` to specify that the filter automatically selects the number of threads. Set to `1` to specify that the filter operates on a single thread.

`alloc_memory`  

The function the filter calls to allocate memory.

`free_memory`  

The function the filter calls to deallocate memory.

## Return Value

A new common filter parameters structure.

## Discussion

If `alloc_memory` is null, BNNS uses `posix_memalign(_:_:_:)` for memory allocation. If free_memory is null, BNNS uses `free()` for memory deallocation.

## See Also

### Initializers

init(options: BNNSFlags, threadCount: Int, allocator: BNNSAlloc?, deallocator: BNNSFree?)

Returns a new common filter parameters structure using the specified options.

init()

