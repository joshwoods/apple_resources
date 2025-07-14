

- Kernel
- Hardware Families
- Mass Storage
- IOCDBlockStorageDriver
-  writeCD 

Instance Method

# writeCD

macOS 10.11.4+

``` source
virtual void writeCD(IOService *client, UInt64 byteStart, IOMemoryDescriptor *buffer, CDSectorArea sectorArea, CDSectorType sectorType, IOStorageAttributes *attributes, IOStorageCompletion *completion);
```

