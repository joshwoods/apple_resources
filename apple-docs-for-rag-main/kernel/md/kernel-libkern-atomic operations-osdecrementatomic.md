

- Kernel
- libkern
- Atomic Operations
-  OSDecrementAtomic 

Function

# OSDecrementAtomic

32-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

macOS 10.0+

``` source
SInt32 OSDecrementAtomic(volatile SInt32 *address);
```

## Parameters 

`address`  

The 4-byte aligned address of the value to update atomically.

## Return Value

The value before the decrement.

## Discussion

The OSDecrementAtomic function decrements the value at the specified address by one and returns the original value.

This function guarantees atomicity only with main system memory. It is specifically unsuitable for use on noncacheable memory such as that in devices; this function cannot guarantee atomicity, for example, on memory mapped from a PCI device. Previous incarnations of this function incorporated a memory barrier on systems with weakly-ordered memory architectures, but current versions contain no barriers.

## See Also

### Decrement

OSDecrementAtomic8

8-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSDecrementAtomic16

16-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSDecrementAtomic64

64-bit decrement.

