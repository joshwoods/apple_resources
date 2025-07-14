

- ImageCaptureCore
- ICCameraItem
-  isRaw 

Instance Property

# isRaw

A Boolean value indicating whether the item is a raw image file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var isRaw: Bool { get }
```

## See Also

### Inspecting an Item’s Name and Type

var uti: String?

The item’s uniform type identifier (UTI) string.

var name: String?

The item’s name.

var ptpObjectHandle: UInt32

The item’s `PTP` object handle value, if the camera uses the `PTP` protocol.

