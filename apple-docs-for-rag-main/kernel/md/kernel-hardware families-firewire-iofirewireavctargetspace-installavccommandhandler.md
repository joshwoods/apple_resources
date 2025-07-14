

- Kernel
- Hardware Families
- FireWire
- IOFireWireAVCTargetSpace
-  installAVCCommandHandler 

Instance Method

# installAVCCommandHandler

macOS 10.11.4+

``` source
virtual IOReturn installAVCCommandHandler(IOFireWireAVCProtocolUserClient *userClient, IOFireWireAVCTargetCommandHandlerCallback callBack, OSAsyncReference64 asyncRef, UInt32 subUnitTypeAndID, UInt32 opCode, uint64_t userCallBack, uint64_t userRefCon);
```

