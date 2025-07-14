

- Accelerate
- BNNSFilterParameters
-  alloc_memory 

Instance Property

# alloc_memory

The function called to allocate memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var alloc_memory: BNNSAlloc?
```

## Discussion

Must be compatible with the free_memory function. If `nil`, `posix_memalign(_:_:_:)` will be called.

## See Also

### Instance Properties

var flags: UInt32

A logical OR of zero or more values from BNNS flags.

var n_threads: Int

The number of worker threads to execute.

var free_memory: BNNSFree?

The function called to deallocate memory.

var allocator: BNNSAlloc?

var deallocator: BNNSFree?

var options: BNNSFlags

var threadCount: Int

