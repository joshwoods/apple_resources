

- ImageCaptureCore
- ICCameraDevice
-  requestDeleteFiles(\_:deleteFailed:completion:) 

Instance Method

# requestDeleteFiles(\_:deleteFailed:completion:)

Deletes files from the camera, with the ability to catch failures and execute a completion block.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func requestDeleteFiles(
    _ files: [ICCameraItem],
    deleteFailed: @escaping ([ICDeleteError : ICCameraItem]) -> Void,
    completion: @escaping ([ICDeleteResult : [ICCameraItem]], (any Error)?) -> Void
) -> Progress?
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

func cancelDelete()

Cancels the current delete operation.

