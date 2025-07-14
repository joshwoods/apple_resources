

- ImageCaptureCore
- ICCameraItem
-  uti 

Instance Property

# uti

The item’s uniform type identifier (UTI) string.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var uti: String? { get }
```

## Discussion

The `UTI` options are `kUTTypeFolder`, `kUTTypeImage`, `kUTTypeMovie`, `kUTTypeAudio`, or `kUTTypeData`.

## See Also

### Inspecting an Item’s Name and Type

var name: String?

The item’s name.

var ptpObjectHandle: UInt32

The item’s `PTP` object handle value, if the camera uses the `PTP` protocol.

var isRaw: Bool

A Boolean value indicating whether the item is a raw image file.

