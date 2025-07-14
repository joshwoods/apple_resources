

- Kernel
- Hardware Families
- FireWire
- IOFireWireAVCTargetSpace
-  addSubunit 

Instance Method

# addSubunit

macOS 10.11.4+

``` source
virtual IOReturn addSubunit(IOFireWireAVCProtocolUserClient *userClient, IOFireWireAVCSubunitPlugHandlerCallback callBack, OSAsyncReference64 asyncRef, UInt32 subunitType, UInt32 numSourcePlugs, UInt32 numDestPlugs, uint64_t userCallBack, uint64_t userRefCon, UInt32 *subUnitID);
```

