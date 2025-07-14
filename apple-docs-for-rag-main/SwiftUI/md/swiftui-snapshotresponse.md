

- SwiftUI
-  SnapshotResponse 

Structure

# SnapshotResponse

Your appplication’s response to a snapshot background task.

watchOS 9.0+

``` source
struct SnapshotResponse
```

## Topics

### Creating a response

init(restoredDefaultState: Bool, estimatedSnapshotExpiration: Date?, identifier: String?)

Creates a snapshot response.

## Relationships

### Conforms To

- Sendable

## See Also

### Handling background tasks

func backgroundTask&lt;D, R>(BackgroundTask&lt;D, R>, action: (D) async -> R) -> some Scene

Runs the specified action when the system provides a background task.

struct BackgroundTask

The kinds of background tasks that your app or extension can handle.

struct SnapshotData

The associated data of a snapshot background task.

