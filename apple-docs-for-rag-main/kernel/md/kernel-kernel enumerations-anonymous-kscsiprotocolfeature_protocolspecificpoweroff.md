

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_ProtocolSpecificPowerOff 

Enumeration Case

# kSCSIProtocolFeature_ProtocolSpecificPowerOff

macOS 10.12+

``` source
kSCSIProtocolFeature_ProtocolSpecificPowerOff = 12
```

## Discussion

If the SCSI Protocol Services Driver supports removing the power to the drive, then the protocol layer should return true. This is used for aggressive power management, specifically for ATAPI devices on ATA buses.

