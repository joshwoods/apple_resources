

- Kernel
- Hardware Families
- FireWire
- IOFireWireNub
-  createWriteQuadCommand 

Instance Method

# createWriteQuadCommand

macOS 10.11.4+

``` source
virtual IOFWWriteQuadCommand * createWriteQuadCommand(FWAddress devAddress, UInt32 *quads, int numQuads, FWDeviceCallback completion, void *refcon, bool failOnReset);
```

