

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  INQUIRY 

Instance Method

# INQUIRY

macOS 10.15.2+

``` source
bool INQUIRY(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit EVPD, SCSICmdField1Byte PAGE_CODE, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

