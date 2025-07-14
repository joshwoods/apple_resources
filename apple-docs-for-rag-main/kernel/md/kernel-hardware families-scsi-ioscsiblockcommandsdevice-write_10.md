

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  WRITE_10 

Instance Method

# WRITE_10

macOS 10.15.2+

``` source
bool WRITE_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField3Bit WRPROTECT, SCSICmdField1Bit DPO, SCSICmdField1Bit FUA, SCSICmdField1Bit FUA_NV, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField2Byte TRANSFER_LENGTH, SCSICmdField1Byte CONTROL);
```

