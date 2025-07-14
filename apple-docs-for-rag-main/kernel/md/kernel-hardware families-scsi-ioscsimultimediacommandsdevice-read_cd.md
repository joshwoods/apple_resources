

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  READ_CD 

Instance Method

# READ_CD

macOS 10.11.4+

``` source
virtual bool READ_CD(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField3Bit EXPECTED_SECTOR_TYPE, SCSICmdField1Bit RELADR, SCSICmdField4Byte STARTING_LOGICAL_BLOCK_ADDRESS, SCSICmdField3Byte TRANSFER_LENGTH, SCSICmdField1Bit SYNC, SCSICmdField2Bit HEADER_CODES, SCSICmdField1Bit USER_DATA, SCSICmdField1Bit EDC_ECC, SCSICmdField2Bit ERROR_FIELD, SCSICmdField3Bit SUBCHANNEL_SELECTION_BITS, SCSICmdField1Byte CONTROL);
```

