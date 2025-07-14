

- ImageCaptureCore
- ICCameraItem
-  parentFolder 

Instance Property

# parentFolder

This item’s parent folder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var parentFolder: ICCameraFolder? { get }
```

## Discussion

The value of this property on the root folder is nil.

## See Also

### Locating an Item

var device: ICCameraDevice?

The item’s parent device.

var fileSystemPath: String?

The item’s file system path on a camera using the mass storage transport type.

var isInTemporaryStore: Bool

A Boolean value that indicates whether this item is in a temporary store.

