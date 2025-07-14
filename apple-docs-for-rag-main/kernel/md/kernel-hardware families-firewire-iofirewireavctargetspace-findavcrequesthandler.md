

- Kernel
- Hardware Families
- FireWire
- IOFireWireAVCTargetSpace
-  findAVCRequestHandler 

Instance Method

# findAVCRequestHandler

macOS 10.11.4+

``` source
virtual IOReturn findAVCRequestHandler(IOFireWireAVCProtocolUserClient *userClient, UInt32 generation, UInt16 nodeID, IOFWSpeed speed, UInt32 handlerSearchIndex, const char *pCmdBuf, UInt32 cmdLen);
```

