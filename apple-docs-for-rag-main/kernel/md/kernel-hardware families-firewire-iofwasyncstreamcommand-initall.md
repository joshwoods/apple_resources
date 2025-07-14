

- Kernel
- Hardware Families
- FireWire
- IOFWAsyncStreamCommand
-  initAll 

Instance Method

# initAll

macOS 10.15.2+

``` source
virtual bool initAll(IOFireWireController *control, UInt32 generation, UInt32 channel, UInt32 sync, UInt32 tag, IOMemoryDescriptor *hostMem, UInt32 size, int speed, FWAsyncStreamCallback completion, void *refcon, bool failOnReset);
```

