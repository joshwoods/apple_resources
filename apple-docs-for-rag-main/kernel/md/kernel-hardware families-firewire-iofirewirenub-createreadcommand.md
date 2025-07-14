

- Kernel
- Hardware Families
- FireWire
- IOFireWireNub
-  createReadCommand 

Instance Method

# createReadCommand

macOS 10.11.4+

``` source
virtual IOFWReadCommand * createReadCommand(FWAddress devAddress, IOMemoryDescriptor *hostMem, FWDeviceCallback completion, void *refcon, bool failOnReset);
```

