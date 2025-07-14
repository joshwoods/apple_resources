

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  READ_DISC_STRUCTURE 

Instance Method

# READ_DISC_STRUCTURE

macOS 10.11.4+

``` source
bool READ_DISC_STRUCTURE(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField4Bit MEDIA_TYPE, SCSICmdField4Byte ADDRESS, SCSICmdField1Byte LAYER_NUMBER, SCSICmdField1Byte FORMAT, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField2Bit AGID, SCSICmdField1Byte CONTROL);
```

