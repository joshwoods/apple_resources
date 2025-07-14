

- SwiftUI
-  SnapshotData 

Structure

# SnapshotData

The associated data of a snapshot background task.

watchOS 9.0+

``` source
struct SnapshotData
```

## Topics

### Getting the data

let identifier: String?

The identifier associated with this snapshot request.

let reason: SnapshotData.SnapshotReason

The reason for a background snapshot task.

enum SnapshotReason

The reason for a background snapshot task.

## Relationships

### Conforms To

- Sendable

## See Also

### Handling background tasks

func backgroundTask&lt;D, R>(BackgroundTask&lt;D, R>, action: (D) async -> R) -> some Scene

Runs the specified action when the system provides a background task.

struct BackgroundTask

The kinds of background tasks that your app or extension can handle.

struct SnapshotResponse

Your appplication’s response to a snapshot background task.

