

- Kernel
- Hardware Families
- FireWire
- IOFireWireController
-  createIsochChannel 

Instance Method

# createIsochChannel

macOS 10.11.4+

``` source
virtual IOFWIsochChannel * createIsochChannel(bool doIRM, UInt32 packetSize, IOFWSpeed prefSpeed, FWIsochChannelForceStopNotificationProc stopProc, void *stopRefCon);
```

