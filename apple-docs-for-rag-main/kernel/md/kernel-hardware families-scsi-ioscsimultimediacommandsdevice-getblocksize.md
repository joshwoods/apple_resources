

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  GetBlockSize 

Instance Method

# GetBlockSize

macOS 10.11.4+

``` source
bool GetBlockSize(UInt32 *requestedByteCount, SCSICmdField3Bit EXPECTED_SECTOR_TYPE, SCSICmdField1Bit SYNC, SCSICmdField2Bit HEADER_CODES, SCSICmdField1Bit USER_DATA, SCSICmdField1Bit EDC_ECC, SCSICmdField2Bit ERROR_FIELD, SCSICmdField3Bit SUBCHANNEL_SELECTION_BITS);
```

