

- Kernel
- Hardware Families
- FireWire
- IOFireWireNub
-  createWriteCommand 

Instance Method

# createWriteCommand

macOS 10.11.4+

``` source
virtual IOFWWriteCommand * createWriteCommand(FWAddress devAddress, IOMemoryDescriptor *hostMem, FWDeviceCallback completion, void *refcon, bool failOnReset);
```

