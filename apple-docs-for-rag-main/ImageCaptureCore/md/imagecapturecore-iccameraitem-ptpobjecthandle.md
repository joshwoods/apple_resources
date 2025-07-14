

- ImageCaptureCore
- ICCameraItem
-  ptpObjectHandle 

Instance Property

# ptpObjectHandle

The item’s `PTP` object handle value, if the camera uses the `PTP` protocol.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var ptpObjectHandle: UInt32 { get }
```

## Discussion

The value of this property is set to `0` if the camera does not use PTP protocol.

## See Also

### Inspecting an Item’s Name and Type

var uti: String?

The item’s uniform type identifier (UTI) string.

var name: String?

The item’s name.

var isRaw: Bool

A Boolean value indicating whether the item is a raw image file.

