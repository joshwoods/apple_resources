

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  PERSISTENT_RESERVE_IN 

Instance Method

# PERSISTENT_RESERVE_IN

macOS 10.11.4+

``` source
virtual bool PERSISTENT_RESERVE_IN(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField5Bit SERVICE_ACTION, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

