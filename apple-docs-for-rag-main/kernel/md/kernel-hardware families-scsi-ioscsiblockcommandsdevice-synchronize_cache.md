

- Kernel
- Hardware Families
- SCSI
- IOSCSIBlockCommandsDevice
-  SYNCHRONIZE_CACHE 

Instance Method

# SYNCHRONIZE_CACHE

macOS 10.15.2+

``` source
bool SYNCHRONIZE_CACHE(SCSITaskIdentifier request, SCSICmdField1Bit IMMED, SCSICmdField1Bit SYNC_NV, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField6Bit GROUP_NUMBER, SCSICmdField2Byte NUMBER_OF_BLOCKS, SCSICmdField1Byte CONTROL);
```

