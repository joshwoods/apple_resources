

- ImageCaptureCore
-  ICDeleteResult 

Structure

# ICDeleteResult

The result of a deletion request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
struct ICDeleteResult
```

## Topics

### Creating a Deletion Result

init(rawValue: String)

### Reading a Deletion Result

static let canceled: ICDeleteResult

The deletion was canceled.

static let failed: ICDeleteResult

The deletion failed.

static let successful: ICDeleteResult

The deletion succeeded.

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

struct ICDeleteError

An error resulting from a deletion request.

func requestDeleteFiles([ICCameraItem])

Deletes files from the camera.

func requestDeleteFiles([ICCameraItem], deleteFailed: ([ICDeleteError : ICCameraItem]) -> Void, completion: ([ICDeleteResult : [ICCameraItem]], (any Error)?) -> Void) -> Progress?

Deletes files from the camera, with the ability to catch failures and execute a completion block.

func cancelDelete()

Cancels the current delete operation.

