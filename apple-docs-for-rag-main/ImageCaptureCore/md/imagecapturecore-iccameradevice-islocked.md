

- ImageCaptureCore
- ICCameraDevice
-  isLocked 

Instance Property

# isLocked

A Boolean value indicating whether the device is locked, preventing deletion of any asset.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var isLocked: Bool { get }
```

## See Also

### Deleting Files

struct ICDeleteResult

The result of a deletion request.

struct ICDeleteError

An error resulting from a deletion request.

func requestDeleteFiles([ICCameraItem])

Deletes files from the camera.

func requestDeleteFiles([ICCameraItem], deleteFailed: ([ICDeleteError : ICCameraItem]) -> Void, completion: ([ICDeleteResult : [ICCameraItem]], (any Error)?) -> Void) -> Progress?

Deletes files from the camera, with the ability to catch failures and execute a completion block.

func cancelDelete()

Cancels the current delete operation.

