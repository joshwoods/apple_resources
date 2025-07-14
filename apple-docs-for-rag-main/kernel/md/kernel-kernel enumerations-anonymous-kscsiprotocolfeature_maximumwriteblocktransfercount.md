

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_MaximumWriteBlockTransferCount 

Enumeration Case

# kSCSIProtocolFeature_MaximumWriteBlockTransferCount

macOS 10.12+

``` source
kSCSIProtocolFeature_MaximumWriteBlockTransferCount = 7
```

## Discussion

If the SCSI Protocol Services Driver has a maximum number of blocks that can be transferred in a write request, it will return true to this query and return the block count in the UInt32 pointer that is passed in as the serviceValue.

