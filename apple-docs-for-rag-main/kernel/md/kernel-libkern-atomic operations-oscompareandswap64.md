

- Kernel
- libkern
- Atomic Operations
-  OSCompareAndSwap64 

Function

# OSCompareAndSwap64

64-bit compare and swap operation.

macOS 10.5+

``` source
Boolean OSCompareAndSwap64(UInt64 oldValue, UInt64 newValue, volatile UInt64 *address);
```

## Discussion

See OSCompareAndSwap.

## See Also

### Compare and Swap

OSCompareAndSwap

Compare and swap operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSCompareAndSwapPtr

Compare and swap operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

