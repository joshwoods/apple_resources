

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  SEND_DIAGNOSTICS 

Instance Method

# SEND_DIAGNOSTICS

macOS 10.11.4+

``` source
virtual bool SEND_DIAGNOSTICS(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField3Bit SELF_TEST_CODE, SCSICmdField1Bit PF, SCSICmdField1Bit SELF_TEST, SCSICmdField1Bit DEVOFFL, SCSICmdField1Bit UNITOFFL, SCSICmdField2Byte PARAMETER_LIST_LENGTH, SCSICmdField1Byte CONTROL);
```

