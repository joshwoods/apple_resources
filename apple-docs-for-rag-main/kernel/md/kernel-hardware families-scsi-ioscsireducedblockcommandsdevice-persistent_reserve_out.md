

- Kernel
- Hardware Families
- SCSI
- IOSCSIReducedBlockCommandsDevice
-  PERSISTENT_RESERVE_OUT 

Instance Method

# PERSISTENT_RESERVE_OUT

macOS 10.11.4+

``` source
virtual bool PERSISTENT_RESERVE_OUT(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField5Bit SERVICE_ACTION, SCSICmdField4Bit SCOPE, SCSICmdField4Bit TYPE);
```

