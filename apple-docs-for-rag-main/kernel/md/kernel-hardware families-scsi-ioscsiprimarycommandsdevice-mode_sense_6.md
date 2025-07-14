

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  MODE_SENSE_6 

Instance Method

# MODE_SENSE_6

macOS 10.11.4+

``` source
virtual bool MODE_SENSE_6(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit DBD, SCSICmdField2Bit PC, SCSICmdField6Bit PAGE_CODE, SCSICmdField1Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

