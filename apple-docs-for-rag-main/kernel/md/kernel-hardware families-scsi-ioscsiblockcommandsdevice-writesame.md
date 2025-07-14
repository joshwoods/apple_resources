

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  WriteSame 

Instance Method

# WriteSame

macOS 10.12+

``` source
virtual IOReturn WriteSame(IOMemoryDescriptor *buffer, UInt64 startBlock, UInt64 blockCount, UInt8 writeSameOptions, UInt32 requestBlockSize);
```

