

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  READ_16 

Instance Method

# READ_16

macOS 10.11.4+

``` source
bool READ_16(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField3Bit RDPROTECT, SCSICmdField1Bit DPO, SCSICmdField1Bit FUA, SCSICmdField1Bit FUA_NV, SCSICmdField8Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField4Byte TRANSFER_LENGTH, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField1Byte CONTROL);
```

