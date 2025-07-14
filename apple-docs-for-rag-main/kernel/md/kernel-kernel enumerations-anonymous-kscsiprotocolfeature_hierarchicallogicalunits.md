

- Kernel
- Kernel Enumerations
- Anonymous
-  kSCSIProtocolFeature_HierarchicalLogicalUnits 

Enumeration Case

# kSCSIProtocolFeature_HierarchicalLogicalUnits

macOS 10.12+

``` source
kSCSIProtocolFeature_HierarchicalLogicalUnits = 15
```

## Discussion

kSCSIProtocolFeature_HierarchicalLogicalUnits: If the SCSI Protocol Services layer supports hierarchical logical units, then the protocol services layer should report true and use IOSCSIProtocolServices::GetLogicalUnitBytes() to retrieve the full 8 bytes of LUN information.

