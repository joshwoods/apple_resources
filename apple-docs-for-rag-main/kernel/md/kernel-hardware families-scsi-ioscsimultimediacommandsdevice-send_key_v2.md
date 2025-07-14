

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  SEND_KEY_V2 

Instance Method

# SEND_KEY_V2

macOS 10.11.4+

``` source
bool SEND_KEY_V2(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Byte KEY_CLASS, SCSICmdField2Byte PARAMETER_LIST_LENGTH, SCSICmdField2Bit AGID, SCSICmdField6Bit KEY_FORMAT, SCSICmdField1Byte CONTROL);
```

