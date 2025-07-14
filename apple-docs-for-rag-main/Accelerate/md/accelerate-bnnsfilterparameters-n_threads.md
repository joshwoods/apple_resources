

- Accelerate
- BNNSFilterParameters
-  n_threads 

Instance Property

# n_threads

The number of worker threads to execute.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var n_threads: Int
```

## Discussion

If `0`, BNNS uses the best number of threads for the current machine.

## See Also

### Instance Properties

var flags: UInt32

A logical OR of zero or more values from BNNS flags.

var alloc_memory: BNNSAlloc?

The function called to allocate memory.

var free_memory: BNNSFree?

The function called to deallocate memory.

var allocator: BNNSAlloc?

var deallocator: BNNSFree?

var options: BNNSFlags

var threadCount: Int

