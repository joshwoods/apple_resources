

- Kernel
- Hardware Families
- SCSI
- IOSCSIReducedBlockCommandsDevice
-  WRITE_10 

Instance Method

# WRITE_10

macOS 10.11.4+

``` source
virtual bool WRITE_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField1Bit FUA, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField2Byte TRANSFER_LENGTH);
```

