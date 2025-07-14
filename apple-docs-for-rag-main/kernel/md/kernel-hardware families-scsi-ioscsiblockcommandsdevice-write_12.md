

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  WRITE_12 

Instance Method

# WRITE_12

macOS 10.15.2+

``` source
bool WRITE_12(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField3Bit WRPROTECT, SCSICmdField1Bit DPO, SCSICmdField1Bit FUA, SCSICmdField1Bit FUA_NV, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField4Byte TRANSFER_LENGTH, SCSICmdField1Byte CONTROL);
```

