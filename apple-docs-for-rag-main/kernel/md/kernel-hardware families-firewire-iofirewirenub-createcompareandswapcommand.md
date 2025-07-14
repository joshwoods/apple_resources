

- Kernel
- Hardware Families
- FireWire
- IOFireWireNub
-  createCompareAndSwapCommand 

Instance Method

# createCompareAndSwapCommand

macOS 10.11.4+

``` source
virtual IOFWCompareAndSwapCommand * createCompareAndSwapCommand(FWAddress devAddress, const UInt32 *cmpVal, const UInt32 *newVal, int size, FWDeviceCallback completion, void *refcon, bool failOnReset);
```

