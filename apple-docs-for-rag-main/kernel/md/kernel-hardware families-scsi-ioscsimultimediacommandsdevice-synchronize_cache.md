

- Kernel
- Hardware Families
- SCSI
- IOSCSIMultimediaCommandsDevice
-  SYNCHRONIZE_CACHE 

Instance Method

# SYNCHRONIZE_CACHE

macOS 10.11.4+

``` source
virtual bool SYNCHRONIZE_CACHE(SCSITaskIdentifier request, SCSICmdField1Bit IMMED, SCSICmdField1Bit RELADR, SCSICmdField4Byte LOGICAL_BLOCK_ADDRESS, SCSICmdField2Byte NUMBER_OF_BLOCKS, SCSICmdField1Byte CONTROL);
```

