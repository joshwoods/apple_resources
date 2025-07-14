

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  READ_DVD_STRUCTURE 

Instance Method

# READ_DVD_STRUCTURE

macOS 10.11.4+

``` source
virtual bool READ_DVD_STRUCTURE(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField4Byte ADDRESS, SCSICmdField1Byte LAYER_NUMBER, SCSICmdField1Byte FORMAT, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField2Bit AGID, SCSICmdField1Byte CONTROL);
```

