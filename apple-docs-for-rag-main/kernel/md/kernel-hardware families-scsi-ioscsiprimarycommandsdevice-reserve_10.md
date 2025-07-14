

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  RESERVE_10 

Instance Method

# RESERVE_10

macOS 10.11.4+

``` source
virtual bool RESERVE_10(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit THRDPTY, SCSICmdField1Bit LONGID, SCSICmdField1Byte THIRD_PARTY_DEVICE_ID, SCSICmdField2Byte PARAMETER_LIST_LENGTH, SCSICmdField1Byte CONTROL);
```

