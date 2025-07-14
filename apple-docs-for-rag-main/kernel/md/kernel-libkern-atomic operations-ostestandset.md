

- Kernel
- libkern
- Atomic Operations
-  OSTestAndSet 

Function

# OSTestAndSet

Bit test and set operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

macOS 10.0+

``` source
Boolean OSTestAndSet(UInt32 bit, volatile UInt8 *startAddress);
```

## Parameters 

`bit`  

The bit number in the range 0 through 7.

`startAddress`  

The address of the byte to update atomically.

## Return Value

true if the bit was already set, false otherwise.

## Discussion

This function guarantees atomicity only with main system memory. It is specifically unsuitable for use on noncacheable memory such as that in devices; this function cannot guarantee atomicity, for example, on memory mapped from a PCI device. Additionally, this function incorporates a memory barrier on systems with weakly-ordered memory architectures.

The OSTestAndSet function sets a single bit in a byte at a specified address. It returns true if the bit was already set, false otherwise.

## See Also

### Test Operations

OSTestAndClear

Bit test and clear operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

