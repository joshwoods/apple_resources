

- Kernel
- libkern
- Atomic Operations
-  OSAddAtomic16 

Function

# OSAddAtomic16

16-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

macOS 10.0+

``` source
SInt16 OSAddAtomic16(SInt32 amount, volatile SInt16 *address);
```

## Parameters 

`address`  

The 2-byte aligned address of the value to update atomically.

## Return Value

The value before the addition

## Discussion

The OSAddAtomic16 function adds the specified amount to the value at the specified address and returns the original value.

This function guarantees atomicity only with main system memory. It is specifically unsuitable for use on noncacheable memory such as that in devices; this function cannot guarantee atomicity, for example, on memory mapped from a PCI device. Previous incarnations of this function incorporated a memory barrier on systems with weakly-ordered memory architectures, but current versions contain no barriers.

## See Also

### Additions

OSAddAtomic

32-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSAddAtomic8

8-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSAddAtomic64

64-bit atomic add operation.

