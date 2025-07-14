

- Kernel
- Hardware Families
- FireWire
- IOFireWireNub
-  createReadQuadCommand 

Instance Method

# createReadQuadCommand

macOS 10.11.4+

``` source
virtual IOFWReadQuadCommand * createReadQuadCommand(FWAddress devAddress, UInt32 *quads, int numQuads, FWDeviceCallback completion, void *refcon, bool failOnReset);
```

