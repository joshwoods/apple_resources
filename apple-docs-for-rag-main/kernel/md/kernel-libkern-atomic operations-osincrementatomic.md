

- Kernel
- libkern
- Atomic Operations
-  OSIncrementAtomic 

Function

# OSIncrementAtomic

32-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

macOS 10.0+

``` source
SInt32 OSIncrementAtomic(volatile SInt32 *address);
```

## Parameters 

`address`  

The 4-byte aligned address of the value to update atomically.

## Return Value

The value before the increment.

## Discussion

The OSIncrementAtomic function increments the value at the specified address by one and returns the original value.

This function guarantees atomicity only with main system memory. It is specifically unsuitable for use on noncacheable memory such as that in devices; this function cannot guarantee atomicity, for example, on memory mapped from a PCI device.

## See Also

### Increment

OSIncrementAtomic8

8-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic16

16-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic64

64-bit increment.

