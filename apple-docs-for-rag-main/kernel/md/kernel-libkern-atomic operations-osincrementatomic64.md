

- Kernel
- libkern
- Atomic Operations
-  OSIncrementAtomic64 

Function

# OSIncrementAtomic64

64-bit increment.

macOS 10.5+

``` source
SInt64 OSIncrementAtomic64(volatile SInt64 *address);
```

## Discussion

See OSIncrementAtomic.

## See Also

### Increment

OSIncrementAtomic

32-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic8

8-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic16

16-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

