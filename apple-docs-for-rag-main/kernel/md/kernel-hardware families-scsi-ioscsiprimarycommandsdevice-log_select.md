

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  LOG_SELECT 

Instance Method

# LOG_SELECT

macOS 10.11.4+

``` source
virtual bool LOG_SELECT(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit PCR, SCSICmdField1Bit SP, SCSICmdField2Bit PC, SCSICmdField2Byte PARAMETER_LIST_LENGTH, SCSICmdField1Byte CONTROL);
```

