

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  GET_CONFIGURATION 

Instance Method

# GET_CONFIGURATION

macOS 10.11.4+

``` source
virtual bool GET_CONFIGURATION(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField2Bit RT, SCSICmdField2Byte STARTING_FEATURE_NUMBER, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

