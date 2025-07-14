

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  READ_TOC_PMA_ATIP 

Instance Method

# READ_TOC_PMA_ATIP

macOS 10.11.4+

``` source
virtual bool READ_TOC_PMA_ATIP(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit MSF, SCSICmdField4Bit FORMAT, SCSICmdField1Byte TRACK_SESSION_NUMBER, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

