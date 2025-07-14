

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_MaximumWriteTransferByteCount 

Enumeration Case

# kSCSIProtocolFeature_MaximumWriteTransferByteCount

macOS 10.12+

``` source
kSCSIProtocolFeature_MaximumWriteTransferByteCount = 9
```

## Discussion

If the SCSI Protocol Services Driver has a maximum byte count that can be transferred in a write request, it will return true to this query and return the byte count in the UInt64 pointer that is passed in as the serviceValue.

