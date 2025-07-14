

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  READ_CD_MSF 

Instance Method

# READ_CD_MSF

macOS 10.11.4+

``` source
virtual bool READ_CD_MSF(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField3Bit EXPECTED_SECTOR_TYPE, SCSICmdField3Byte STARTING_MSF, SCSICmdField3Byte ENDING_MSF, SCSICmdField1Bit SYNC, SCSICmdField2Bit HEADER_CODES, SCSICmdField1Bit USER_DATA, SCSICmdField1Bit EDC_ECC, SCSICmdField2Bit ERROR_FIELD, SCSICmdField3Bit SUBCHANNEL_SELECTION_BITS, SCSICmdField1Byte CONTROL);
```

