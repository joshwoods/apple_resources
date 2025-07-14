

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  READ_12 

Instance Method

# READ_12

macOS 10.15.2+

``` source
bool READ_12(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField3Bit RDPROTECT, SCSICmdField1Bit DPO, SCSICmdField1Bit FUA, SCSICmdField1Bit FUA_NV, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField4Byte TRANSFER_LENGTH, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField1Byte CONTROL);
```

