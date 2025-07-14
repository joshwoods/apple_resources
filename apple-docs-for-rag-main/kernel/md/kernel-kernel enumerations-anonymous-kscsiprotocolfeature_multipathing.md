

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_MultiPathing 

Enumeration Case

# kSCSIProtocolFeature_MultiPathing

macOS 10.12+

``` source
kSCSIProtocolFeature_MultiPathing = 16
```

## Discussion

kSCSIProtocolFeature_MultiPathing: If the SCSI Protocol Services layer supports multi-pathing, then the protocol services layer should report true. This is used to support multiple paths to a logical unit by creating a IOSCSIMultipathedLogicalUnit object.

