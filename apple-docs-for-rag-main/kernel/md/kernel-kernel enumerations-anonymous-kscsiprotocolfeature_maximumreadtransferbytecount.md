

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_MaximumReadTransferByteCount 

Enumeration Case

# kSCSIProtocolFeature_MaximumReadTransferByteCount

macOS 10.12+

``` source
kSCSIProtocolFeature_MaximumReadTransferByteCount = 8
```

## Discussion

If the SCSI Protocol Services Driver has a maximum byte count that can be transferred in a read request, it will return true to this query and return the byte count in the UInt64 pointer that is passed in as the serviceValue.

