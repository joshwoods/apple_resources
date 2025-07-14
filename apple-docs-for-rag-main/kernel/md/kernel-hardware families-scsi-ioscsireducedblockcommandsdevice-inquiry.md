

- Kernel
- Hardware Families
- SCSI
- IOSCSIReducedBlockCommandsDevice
-  INQUIRY 

Instance Method

# INQUIRY

macOS 10.11.4+

``` source
virtual bool INQUIRY(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit CMDDT, SCSICmdField1Bit EVPD, SCSICmdField1Byte PAGE_OR_OPERATION_CODE, SCSICmdField1Byte ALLOCATION_LENGTH);
```

