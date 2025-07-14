

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  WRITE_BUFFER 

Instance Method

# WRITE_BUFFER

macOS 10.11.4+

``` source
virtual bool WRITE_BUFFER(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField4Bit MODE, SCSICmdField1Byte BUFFER_ID, SCSICmdField3Byte BUFFER_OFFSET, SCSICmdField3Byte PARAMETER_LIST_LENGTH, SCSICmdField1Byte CONTROL);
```

