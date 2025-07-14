

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  readCD 

Instance Method

# readCD

macOS 10.15.2+

``` source
virtual IOReturn readCD(IOService *client, UInt64 byteStart, IOMemoryDescriptor *buffer, CDSectorArea sectorArea, CDSectorType sectorType, IOStorageAttributes *attributes, UInt64 *actualByteCount);
```

