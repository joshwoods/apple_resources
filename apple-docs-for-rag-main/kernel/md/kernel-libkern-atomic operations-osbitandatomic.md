

- Kernel
- libkern
- Atomic Operations
-  OSBitAndAtomic 

Function

# OSBitAndAtomic

32-bit logical and operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

macOS 10.0+

``` source
UInt32 OSBitAndAtomic(UInt32 mask, volatile UInt32 *address);
```

## Parameters 

`mask`  

The mask to logically and with the value.

`address`  

The 4-byte aligned address of the value to update atomically.

## Return Value

The value before the bitwise operation

## Discussion

The OSBitAndAtomic function logically ands the bits of the specified mask into the value at the specified address and returns the original value.

This function guarantees atomicity only with main system memory. It is specifically unsuitable for use on noncacheable memory such as that in devices; this function cannot guarantee atomicity, for example, on memory mapped from a PCI device. Previous incarnations of this function incorporated a memory barrier on systems with weakly-ordered memory architectures, but current versions contain no barriers..

## See Also

### Boolean Operations

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

OSBitXorAtomic

32-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitXorAtomic8

8-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitXorAtomic16

16-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

