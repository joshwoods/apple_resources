

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_GetMaximumLogicalUnitNumber 

Enumeration Case

# kSCSIProtocolFeature_GetMaximumLogicalUnitNumber

macOS 10.12+

``` source
kSCSIProtocolFeature_GetMaximumLogicalUnitNumber = 5
```

## Discussion

If the SCSI Protocol Services Driver supports logical units, it will report the maximum addressable ID that it supports in the UInt32 pointer that is passed in as the serviceValue. If only one unit is supported, the driver should return false for this query.

