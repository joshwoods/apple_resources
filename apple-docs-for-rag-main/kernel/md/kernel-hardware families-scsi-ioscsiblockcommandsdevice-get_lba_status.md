

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  GET_LBA_STATUS 

Instance Method

# GET_LBA_STATUS

macOS 10.12+

``` source
bool GET_LBA_STATUS(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField8Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField4Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

