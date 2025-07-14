

- Kernel
- Hardware Families
- FireWire
- IOFireWireController
-  asyncWrite 

Instance Method

# asyncWrite

macOS 10.15.2+

``` source
virtual IOReturn asyncWrite(UInt32 generation, UInt16 nodeID, UInt16 addrHi, UInt32 addrLo, int speed, int label, void *data, int size, IOFWAsyncCommand *cmd);
```

