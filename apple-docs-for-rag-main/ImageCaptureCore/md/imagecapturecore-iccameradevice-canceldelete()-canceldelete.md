

- ImageCaptureCore
- ICCameraDevice
-  cancelDelete() 

Instance Method

# cancelDelete()

Cancels the current delete operation.

macOS 10.4+

``` source
func cancelDelete()
```

## See Also

### Deleting Files

var isLocked: Bool

A Boolean value indicating whether the device is locked, preventing deletion of any asset.

struct ICDeleteResult

The result of a deletion request.

struct ICDeleteError

An error resulting from a deletion request.

func requestDeleteFiles([ICCameraItem])

Deletes files from the camera.

func requestDeleteFiles([ICCameraItem], deleteFailed: ([ICDeleteError : ICCameraItem]) -> Void, completion: ([ICDeleteResult : [ICCameraItem]], (any Error)?) -> Void) -> Progress?

Deletes files from the camera, with the ability to catch failures and execute a completion block.

