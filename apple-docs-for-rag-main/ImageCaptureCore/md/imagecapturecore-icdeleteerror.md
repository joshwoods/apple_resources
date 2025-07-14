

- ImageCaptureCore
-  ICDeleteError 

Structure

# ICDeleteError

An error resulting from a deletion request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
struct ICDeleteError
```

## Topics

### Creating a Deletion Error

init(rawValue: String)

### Reading a Deletion Error

static let canceled: ICDeleteError

The deletion was canceled.

static let deviceMissing: ICDeleteError

The deletion failed because the device could not be found.

static let fileMissing: ICDeleteError

The deletion failed because the file could not be found.

static let readOnly: ICDeleteError

The deletion failed because the file had read-only permissions.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deleting Files

var isLocked: Bool

A Boolean value indicating whether the device is locked, preventing deletion of any asset.

struct ICDeleteResult

The result of a deletion request.

func requestDeleteFiles([ICCameraItem])

Deletes files from the camera.

func requestDeleteFiles([ICCameraItem], deleteFailed: ([ICDeleteError : ICCameraItem]) -> Void, completion: ([ICDeleteResult : [ICCameraItem]], (any Error)?) -> Void) -> Progress?

Deletes files from the camera, with the ability to catch failures and execute a completion block.

func cancelDelete()

Cancels the current delete operation.

