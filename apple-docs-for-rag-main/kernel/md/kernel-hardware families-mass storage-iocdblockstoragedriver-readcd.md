

- Kernel
- Hardware Families
- Mass Storage
- IOCDBlockStorageDriver
-  readCD 

Instance Method

# readCD

macOS 10.11.4+

``` source
virtual void readCD(IOService *client, UInt64 byteStart, IOMemoryDescriptor *buffer, CDSectorArea sectorArea, CDSectorType sectorType, IOStorageAttributes *attributes, IOStorageCompletion *completion);
```

