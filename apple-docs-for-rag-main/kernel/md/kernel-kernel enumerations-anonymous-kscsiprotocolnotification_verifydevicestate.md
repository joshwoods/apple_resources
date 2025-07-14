

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolNotification_VerifyDeviceState 

Enumeration Case

# kSCSIProtocolNotification_VerifyDeviceState

macOS 10.12+

``` source
kSCSIProtocolNotification_VerifyDeviceState = 0x69000020
```

## Discussion

Private message sent between a SCSI protocol service provider and SCSI application layer driver to indicate device state may have changed and the device state should be re-verified by the SCSI Application Layer driver. An example would be a bus reset which clears the tray locking state of an ATAPI device.

