

- Kernel
- Hardware Families
- FireWire
- IOFireWireController
-  createAsyncStreamCommand 

Instance Method

# createAsyncStreamCommand

macOS 10.15.2+

``` source
virtual IOFWAsyncStreamCommand * createAsyncStreamCommand(UInt32 generation, UInt32 channel, UInt32 sync, UInt32 tag, IOMemoryDescriptor *hostMem, UInt32 size, int speed, FWAsyncStreamCallback completion, void *refcon, bool failOnReset);
```

