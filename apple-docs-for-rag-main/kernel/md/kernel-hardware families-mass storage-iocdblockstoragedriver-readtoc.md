

- Kernel
- Hardware Families
- Mass Storage
- IOCDBlockStorageDriver
-  readTOC 

Instance Method

# readTOC

macOS 10.11.4+

``` source
virtual IOReturn readTOC(IOMemoryDescriptor *buffer, CDTOCFormat format, UInt8 formatAsTime, UInt8 trackOrSessionNumber, UInt16 *actualByteCount);
```

