

- Kernel
- libkern
- Atomic Operations
-  OSIncrementAtomic8 

Function

# OSIncrementAtomic8

8-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

macOS 10.0+

``` source
SInt8 OSIncrementAtomic8(volatile SInt8 *address);
```

## Parameters 

`address`  

The address of the value to update atomically.

## Return Value

The value before the increment.

## Discussion

The OSIncrementAtomic8 function increments the value at the specified address by one and returns the original value.

This function guarantees atomicity only with main system memory. It is specifically unsuitable for use on noncacheable memory such as that in devices; this function cannot guarantee atomicity, for example, on memory mapped from a PCI device. Previous incarnations of this function incorporated a memory barrier on systems with weakly-ordered memory architectures, but current versions contain no barriers.

## See Also

### Increment

OSIncrementAtomic

32-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic16

16-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic64

64-bit increment.

