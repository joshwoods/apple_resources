

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  READ_CAPACITY 

Instance Method

# READ_CAPACITY

macOS 10.11.4+

``` source
virtual bool READ_CAPACITY(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit RELADR, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField1Bit PMI, SCSICmdField1Byte CONTROL);
```

