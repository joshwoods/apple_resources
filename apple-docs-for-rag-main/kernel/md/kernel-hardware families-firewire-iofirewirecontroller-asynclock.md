

- Kernel
- Hardware Families
- FireWire
- IOFireWireController
-  asyncLock 

Instance Method

# asyncLock

macOS 10.15.2+

``` source
virtual IOReturn asyncLock(UInt32 generation, UInt16 nodeID, UInt16 addrHi, UInt32 addrLo, int speed, int label, int type, IOMemoryDescriptor *buf, IOByteCount offset, int size, IOFWAsyncCommand *cmd);
```

