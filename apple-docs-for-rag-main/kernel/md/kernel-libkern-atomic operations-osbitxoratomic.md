

- Kernel
- libkern
- Atomic Operations
-  OSBitXorAtomic 

Function

# OSBitXorAtomic

32-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

macOS 10.0+

``` source
UInt32 OSBitXorAtomic(UInt32 mask, volatile UInt32 *address);
```

## Parameters 

`mask`  

The mask to logically or with the value.

`address`  

The 4-byte aligned address of the value to update atomically.

## Return Value

The value before the bitwise operation.

## Discussion

This function guarantees atomicity only with main system memory. It is specifically unsuitable for use on noncacheable memory such as that in devices; this function cannot guarantee atomicity, for example, on memory mapped from a PCI device. Additionally, this function incorporates a memory barrier on systems with weakly-ordered memory architectures.

The OSBitXorAtomic function logically xors the bits of the specified mask into the value at the specified address and returns the original value.

## See Also

### Boolean Operations

OSBitAndAtomic

32-bit logical and operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitAndAtomic8

8-bit logical and operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitAndAtomic16

16-bit logical and operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitOrAtomic

32-bit logical or operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitOrAtomic8

8-bit logical or operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitOrAtomic16

16-bit logical or operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitXorAtomic8

8-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitXorAtomic16

16-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

