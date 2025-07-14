

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  WRITE_SAME_10 

Instance Method

# WRITE_SAME_10

macOS 10.12+

``` source
bool WRITE_SAME_10(SCSITaskIdentifier request, IOMemoryDescriptor *buffer, UInt32 requestBlockSize, SCSICmdField3Bit WRPROTECT, SCSICmdField1Bit ANCHOR, SCSICmdField1Bit UNMAP, SCSICmdField4Byte startBlock, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField2Byte blockCount, SCSICmdField1Byte CONTROL);
```

