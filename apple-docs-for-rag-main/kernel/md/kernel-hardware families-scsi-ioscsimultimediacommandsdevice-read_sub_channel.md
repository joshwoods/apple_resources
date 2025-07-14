

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  READ_SUB_CHANNEL 

Instance Method

# READ_SUB_CHANNEL

macOS 10.11.4+

``` source
virtual bool READ_SUB_CHANNEL(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit MSF, SCSICmdField1Bit SUBQ, SCSICmdField1Byte SUB_CHANNEL_PARAMETER_LIST, SCSICmdField1Byte TRACK_NUMBER, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

