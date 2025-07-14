

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  WRITE_16 

Instance Method

# WRITE_16

macOS 10.11.4+

``` source
bool WRITE_16(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField3Bit WRPROTECT, SCSICmdField1Bit DPO, SCSICmdField1Bit FUA, SCSICmdField1Bit FUA_NV, SCSICmdField8Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField4Byte TRANSFER_LENGTH, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField1Byte CONTROL);
```

