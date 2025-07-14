

- Kernel
- Hardware Families
- FireWire
- IOFireWireController
-  asyncStreamWrite 

Instance Method

# asyncStreamWrite

macOS 10.11.4+

``` source
virtual IOReturn asyncStreamWrite(UInt32 generation, int speed, int tag, int sync, int channel, IOMemoryDescriptor *buf, IOByteCount offset, int size, IOFWAsyncStreamCommand *cmd);
```

