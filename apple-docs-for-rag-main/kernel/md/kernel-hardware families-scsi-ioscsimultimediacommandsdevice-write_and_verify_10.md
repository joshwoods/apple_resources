

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  WRITE_AND_VERIFY_10 

Instance Method

# WRITE_AND_VERIFY_10

macOS 10.11.4+

``` source
virtual bool WRITE_AND_VERIFY_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, UInt32 blockSize, SCSICmdField1Bit DPO, SCSICmdField1Bit BYT_CHK, SCSICmdField1Bit RELADR, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField4Byte TRANSFER_LENGTH, SCSICmdField1Byte CONTROL);
```

