

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  GET_PERFORMANCE 

Instance Method

# GET_PERFORMANCE

macOS 10.11.4+

``` source
virtual bool GET_PERFORMANCE(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField2Bit TOLERANCE, SCSICmdField1Bit WRITE, SCSICmdField2Bit EXCEPT, SCSICmdField4Byte STARTING_LBA, SCSICmdField2Byte MAXIMUM_NUMBER_OF_DESCRIPTORS, SCSICmdField1Byte CONTROL);
```

