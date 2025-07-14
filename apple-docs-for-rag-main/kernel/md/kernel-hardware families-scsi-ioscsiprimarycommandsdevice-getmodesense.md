

- Kernel
- Hardware Families
- SCSI
- IOSCSIPrimaryCommandsDevice
-  GetModeSense 

Instance Method

# GetModeSense

macOS 10.11.4+

``` source
IOReturn GetModeSense(IOMemoryDescriptor *dataBuffer, SCSICmdField6Bit PAGE_CODE, SCSICmdField2Byte ALLOCATION_LENGTH, bool *use10ByteModeSense);
```

