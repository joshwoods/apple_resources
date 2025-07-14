

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  READ_10 

Instance Method

# READ_10

macOS 10.11.4+

``` source
virtual bool READ_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField1Bit DPO, SCSICmdField1Bit FUA, SCSICmdField1Bit RELADR, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField2Byte TRANSFER_LENGTH, SCSICmdField1Byte CONTROL);
```

