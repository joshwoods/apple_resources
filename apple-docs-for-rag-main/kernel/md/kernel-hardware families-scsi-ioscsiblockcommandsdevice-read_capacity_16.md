

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  READ_CAPACITY_16 

Instance Method

# READ_CAPACITY_16

macOS 10.11.4+

``` source
bool READ_CAPACITY_16(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField8Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField4Byte ALLOCATION_LENGTH, SCSICmdField1Bit PMI, SCSICmdField1Byte CONTROL);
```

