

- AVFoundation
- AVExternalStorageDevice
-  isNotRecommendedForCaptureUse 

Instance Property

# isNotRecommendedForCaptureUse

A Boolean value that indicates whether the external storage device is suitable for camera capture.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var isNotRecommendedForCaptureUse: Bool { get }
```

## See Also

### Inspecting a storage device

var isConnected: Bool

A Boolean value that indicates whether the system has a connection to the external storage device.

var displayName: String?

The name of an external storage device that’s appropriate for a user interface.

var uuid: UUID?

The external storage device’s unique identifier.

var freeSize: Int

The amount of free storage space, in bytes, that’s available on the external storage device.

var totalSize: Int

The total amount of storage space, in bytes, that’s available on the external storage device.

