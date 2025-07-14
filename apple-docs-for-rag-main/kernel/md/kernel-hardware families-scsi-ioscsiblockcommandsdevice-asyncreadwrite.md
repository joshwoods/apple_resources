

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  AsyncReadWrite 

Instance Method

# AsyncReadWrite

macOS 10.15.2+

``` source
virtual IOReturn AsyncReadWrite(IOMemoryDescriptor *buffer, UInt64 startBlock, UInt64 blockCount, UInt64 blockSize, IOStorageAttributes *attributes, void *clientData);
```

