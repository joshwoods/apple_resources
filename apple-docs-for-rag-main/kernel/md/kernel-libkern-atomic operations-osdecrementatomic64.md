

- Kernel
- libkern
- Atomic Operations
-  OSDecrementAtomic64 

Function

# OSDecrementAtomic64

64-bit decrement.

macOS 10.5+

``` source
SInt64 OSDecrementAtomic64(volatile SInt64 *address);
```

## Discussion

See OSDecrementAtomic.

## See Also

### Decrement

OSDecrementAtomic

32-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSDecrementAtomic8

8-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSDecrementAtomic16

16-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

