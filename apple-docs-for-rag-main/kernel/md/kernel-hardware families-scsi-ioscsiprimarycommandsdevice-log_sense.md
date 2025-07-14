

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  LOG_SENSE 

Instance Method

# LOG_SENSE

macOS 10.11.4+

``` source
virtual bool LOG_SENSE(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit PPC, SCSICmdField1Bit SP, SCSICmdField2Bit PC, SCSICmdField6Bit PAGE_CODE, SCSICmdField2Byte PARAMETER_POINTER, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

