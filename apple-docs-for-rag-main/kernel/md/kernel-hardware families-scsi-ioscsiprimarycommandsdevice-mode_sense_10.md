

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  MODE_SENSE_10 

Instance Method

# MODE_SENSE_10

macOS 10.11.4+

``` source
virtual bool MODE_SENSE_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit LLBAA, SCSICmdField1Bit DBD, SCSICmdField2Bit PC, SCSICmdField6Bit PAGE_CODE, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

