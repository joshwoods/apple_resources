

- Accelerate
- BNNSFilterParameters
-  free_memory 

Instance Property

# free_memory

The function called to deallocate memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var free_memory: BNNSFree?
```

## Discussion

Must be compatible with the alloc_memory function. If `nil`, `free()` will be called.

## See Also

### Instance Properties

var flags: UInt32

A logical OR of zero or more values from BNNS flags.

var n_threads: Int

The number of worker threads to execute.

var alloc_memory: BNNSAlloc?

The function called to allocate memory.

var allocator: BNNSAlloc?

var deallocator: BNNSFree?

var options: BNNSFlags

var threadCount: Int

