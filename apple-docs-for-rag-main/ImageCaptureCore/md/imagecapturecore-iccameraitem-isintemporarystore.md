

- ImageCaptureCore
- ICCameraItem
-  isInTemporaryStore 

Instance Property

# isInTemporaryStore

A Boolean value that indicates whether this item is in a temporary store.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var isInTemporaryStore: Bool { get }
```

## Discussion

A device may use a temporary store when it captures images while tethered to a computer.

## See Also

### Locating an Item

var device: ICCameraDevice?

The item’s parent device.

var fileSystemPath: String?

The item’s file system path on a camera using the mass storage transport type.

var parentFolder: ICCameraFolder?

This item’s parent folder.

