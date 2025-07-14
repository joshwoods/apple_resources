

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  WRITE_SAME_16 

Instance Method

# WRITE_SAME_16

macOS 10.12+

``` source
bool WRITE_SAME_16(SCSITaskIdentifier request, IOMemoryDescriptor *buffer, UInt32 requestBlockSize, SCSICmdField3Bit WRPROTECT, SCSICmdField1Bit ANCHOR, SCSICmdField1Bit UNMAP, SCSICmdField1Bit NDOB, SCSICmdField8Byte startBlock, SCSICmdField4Byte blockCount, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField1Byte CONTROL);
```

