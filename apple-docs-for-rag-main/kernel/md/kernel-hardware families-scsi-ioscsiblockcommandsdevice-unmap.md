

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  UNMAP 

Instance Method

# UNMAP

macOS 10.12+

``` source
bool UNMAP(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit ANCHOR, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField2Byte PARAMETER_LIST_LENGTH, SCSICmdField1Byte CONTROL);
```

