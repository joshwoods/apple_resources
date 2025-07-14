

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  REPORT_KEY_V3 

Instance Method

# REPORT_KEY_V3

macOS 10.12+

``` source
bool REPORT_KEY_V3(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField1Byte KEY_CLASS, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte BLOCK_COUNT, SCSICmdField2Bit AGID, SCSICmdField6Bit KEY_FORMAT, SCSICmdField1Byte CONTROL);
```

