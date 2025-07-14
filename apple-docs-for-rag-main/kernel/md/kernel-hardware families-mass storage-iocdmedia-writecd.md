

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  writeCD 

Instance Method

# writeCD

macOS 10.15.2+

``` source
virtual IOReturn writeCD(IOService *client, UInt64 byteStart, IOMemoryDescriptor *buffer, CDSectorArea sectorArea, CDSectorType sectorType, IOStorageAttributes *attributes, UInt64 *actualByteCount);
```

