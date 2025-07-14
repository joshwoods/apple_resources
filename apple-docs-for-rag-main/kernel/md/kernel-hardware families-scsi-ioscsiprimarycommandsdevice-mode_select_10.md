

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  MODE_SELECT_10 

Instance Method

# MODE_SELECT_10

macOS 10.11.4+

``` source
virtual bool MODE_SELECT_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit PF, SCSICmdField1Bit SP, SCSICmdField2Byte PARAMETER_LIST_LENGTH, SCSICmdField1Byte CONTROL);
```

