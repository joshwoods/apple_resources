

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_ProtocolSpecificAsyncNotification 

Enumeration Case

# kSCSIProtocolFeature_ProtocolSpecificAsyncNotification

macOS 10.12+

``` source
kSCSIProtocolFeature_ProtocolSpecificAsyncNotification = 14
```

## Discussion

Used to determine if the SCSI Protocol Services Driver supports asynchronous notifications from the drive. This is used to prevent polling for media, specifically for SATAPI devices on AHCI buses.

