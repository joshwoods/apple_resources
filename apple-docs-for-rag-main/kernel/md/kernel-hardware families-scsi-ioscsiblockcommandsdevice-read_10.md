

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  READ_10 

Instance Method

# READ_10

macOS 10.15.2+

``` source
bool READ_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField3Bit RDPROTECT, SCSICmdField1Bit DPO, SCSICmdField1Bit FUA, SCSICmdField1Bit FUA_NV, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField2Byte TRANSFER_LENGTH, SCSICmdField1Byte CONTROL);
```

