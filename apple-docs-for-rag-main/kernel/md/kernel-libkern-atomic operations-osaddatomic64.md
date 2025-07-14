

- Kernel
- libkern
- Atomic Operations
-  OSAddAtomic64 

Function

# OSAddAtomic64

64-bit atomic add operation.

macOS 10.5+

``` source
SInt64 OSAddAtomic64(SInt64 theAmount, volatile SInt64 *address);
```

## Discussion

See OSAddAtomic.

## See Also

### Additions

OSAddAtomic

32-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSAddAtomic8

8-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSAddAtomic16

16-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

