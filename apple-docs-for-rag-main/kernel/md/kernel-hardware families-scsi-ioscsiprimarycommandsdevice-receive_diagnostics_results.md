

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  RECEIVE_DIAGNOSTICS_RESULTS 

Instance Method

# RECEIVE_DIAGNOSTICS_RESULTS

macOS 10.11.4+

``` source
virtual bool RECEIVE_DIAGNOSTICS_RESULTS(SCSITaskIdentifier request, IOMemoryDescriptor *dataBuffer, SCSICmdField1Bit PCV, SCSICmdField1Byte PAGE_CODE, SCSICmdField2Byte ALLOCATION_LENGTH, SCSICmdField1Byte CONTROL);
```

