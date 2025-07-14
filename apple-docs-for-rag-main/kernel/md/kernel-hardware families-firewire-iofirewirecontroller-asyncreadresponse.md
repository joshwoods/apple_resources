

- Kernel
- Hardware Families
- FireWire
- IOFireWireController
-  asyncReadResponse 

Instance Method

# asyncReadResponse

macOS 10.11.4+

``` source
virtual IOReturn asyncReadResponse(UInt32 generation, UInt16 nodeID, int speed, IOMemoryDescriptor *buf, IOByteCount offset, int len, IOFWRequestRefCon refcon);
```

