

- Kernel
- Hardware Families
- SCSI
- IOSCSIReducedBlockCommandsDevice
-  READ_10 

Instance Method

# READ_10

macOS 10.11.4+

``` source
virtual bool READ_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField2Byte TRANSFER_LENGTH);
```

