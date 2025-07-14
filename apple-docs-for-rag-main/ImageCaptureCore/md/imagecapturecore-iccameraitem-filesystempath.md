

- ImageCaptureCore
- ICCameraItem
-  fileSystemPath 

Instance Property

# fileSystemPath

The item’s file system path on a camera using the mass storage transport type.

macOS 10.4+

``` source
var fileSystemPath: String? { get }
```

## Discussion

This property is set for cameras whose transportType is transportTypeMassStorage.

## See Also

### Locating an Item

var device: ICCameraDevice?

The item’s parent device.

var parentFolder: ICCameraFolder?

This item’s parent folder.

var isInTemporaryStore: Bool

A Boolean value that indicates whether this item is in a temporary store.

