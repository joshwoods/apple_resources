

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_ProtocolAlwaysReportsAutosenseData 

Enumeration Case

# kSCSIProtocolFeature_ProtocolAlwaysReportsAutosenseData

macOS 10.12+

``` source
kSCSIProtocolFeature_ProtocolAlwaysReportsAutosenseData = 11
```

## Discussion

If the SCSI Protocol Services Driver always reports available autosense data when a kSCSITaskStatus_CHECK_CONDITION is set, then the protocol layer should return true. E.g. FireWire transport drivers should respond true to this.

