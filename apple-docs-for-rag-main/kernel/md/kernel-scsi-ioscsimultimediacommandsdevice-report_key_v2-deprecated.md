

- Kernel
- Hardware Families
- 
  - Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  REPORT_KEY_V2 Deprecated

Instance Method

# REPORT_KEY_V2

macOS 10.11.4–10.12Deprecated

``` source
bool REPORT_KEY_V2(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField1Byte KEY_CLASS, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField2Bit AGID, SCSICmdField6Bit KEY_FORMAT, SCSICmdField1Byte CONTROL);
```

