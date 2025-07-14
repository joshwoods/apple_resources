

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  READ_TRACK_INFORMATION 

Instance Method

# READ_TRACK_INFORMATION

macOS 10.11.4+

``` source
virtual bool READ_TRACK_INFORMATION(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField2Bit ADDRESS_NUMBER_TYPE, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS_TRACK_SESSION_NUMBER, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

