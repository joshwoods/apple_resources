

- Core Services
- File Metadata
- MDItem
- Common Metadata Attribute Keys
-  kMDItemRights 

Global Variable

# kMDItemRights

Provides a link to information about rights held in and over the resource. A CFString.

macOS 10.4+

``` source
let kMDItemRights: CFString!
```

## Discussion

Contains a rights management statement for the resource, or reference a service providing such information. Rights information often encompasses Intellectual Property Rights (IPR), Copyright, and various Property Rights.

If this attribute is absent, no assumptions can be made about the status of these and other rights with respect to the resource.

