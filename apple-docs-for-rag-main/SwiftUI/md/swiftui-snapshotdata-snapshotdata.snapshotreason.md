

- SwiftUI
- SnapshotData
-  SnapshotData.SnapshotReason 

Enumeration

# SnapshotData.SnapshotReason

The reason for a background snapshot task.

watchOS 9.0+

``` source
enum SnapshotReason
```

## Topics

### Getting the snapshot reasons

case appBackgrounded

The app transitioned from the foreground to the background.

case appScheduled

The app scheduled this snapshot.

case complicationUpdate

The app updated the complication timeline.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

case returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the data

let identifier: String?

The identifier associated with this snapshot request.

let reason: SnapshotData.SnapshotReason

The reason for a background snapshot task.

