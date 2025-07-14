

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  SEND 

Instance Method

# SEND

macOS 10.11.4+

``` source
virtual bool SEND(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit AER, SCSICmdField3Byte TRANSFER_LENGTH, SCSICmdField1Byte CONTROL);
```

