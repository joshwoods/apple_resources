

- FSKit
- FSExtentPacker
-  packExtent(resource:type:logicalOffset:physicalOffset:length:) 

Instance Method

# packExtent(resource:type:logicalOffset:physicalOffset:length:)

Packs a single extent to send to the kernel.

macOS 15.4+

``` source
func packExtent(
    resource: FSBlockDeviceResource,
    type: FSExtentType,
    logicalOffset: off_t,
    physicalOffset: off_t,
    length: Int
) -> Bool
```

## Parameters 

`resource`  

The resource on which to perform I/O.

`type`  

The type of extent, indicating whether it contains valid data.

`logicalOffset`  

The extent offset within the file, in bytes.

`physicalOffset`  

The extent offset on disk, in bytes.

`length`  

The extent length, in bytes.

## Return Value

A Boolean value that indicates whether the packer can pack more extents.

## See Also

### Packing extents

enum FSExtentType

An enumeration of types of extents.

