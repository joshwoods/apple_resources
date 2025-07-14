

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  READ_BUFFER 

Instance Method

# READ_BUFFER

macOS 10.11.4+

``` source
virtual bool READ_BUFFER(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField4Bit MODE, SCSICmdField1Byte BUFFER_ID, SCSICmdField3Byte BUFFER_OFFSET, SCSICmdField3Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

