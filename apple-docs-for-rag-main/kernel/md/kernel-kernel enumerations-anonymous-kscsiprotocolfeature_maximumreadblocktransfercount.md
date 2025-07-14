

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_MaximumReadBlockTransferCount 

Enumeration Case

# kSCSIProtocolFeature_MaximumReadBlockTransferCount

macOS 10.12+

``` source
kSCSIProtocolFeature_MaximumReadBlockTransferCount = 6
```

## Discussion

If the SCSI Protocol Services Driver has a maximum number of blocks that can be transfered in a read request, it will return true to this query and return the block count in the UInt32 pointer that is passed in as the serviceValue.

