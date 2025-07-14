

- Kernel
- Hardware Families
- FireWire
- IOFireWireController
-  asyncLockResponse 

Instance Method

# asyncLockResponse

macOS 10.11.4+

``` source
virtual IOReturn asyncLockResponse(UInt32 generation, UInt16 nodeID, int speed, IOMemoryDescriptor *buf, IOByteCount offset, int len, IOFWRequestRefCon refcon);
```

