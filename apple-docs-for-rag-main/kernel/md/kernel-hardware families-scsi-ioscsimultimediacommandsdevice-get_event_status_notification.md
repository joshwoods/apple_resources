

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  GET_EVENT_STATUS_NOTIFICATION 

Instance Method

# GET_EVENT_STATUS_NOTIFICATION

macOS 10.11.4+

``` source
virtual bool GET_EVENT_STATUS_NOTIFICATION(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit IMMED, SCSICmdField1Byte NOTIFICATION_CLASS_REQUEST, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

