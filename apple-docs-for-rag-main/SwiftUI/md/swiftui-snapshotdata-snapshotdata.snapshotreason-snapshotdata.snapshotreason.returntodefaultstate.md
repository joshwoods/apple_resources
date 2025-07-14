

- SwiftUI
- SnapshotData
- SnapshotData.SnapshotReason
-  SnapshotData.SnapshotReason.returnToDefaultState 

Case

# SnapshotData.SnapshotReason.returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

watchOS 9.0+

``` source
case returnToDefaultState
```

## See Also

### Getting the snapshot reasons

case appBackgrounded

The app transitioned from the foreground to the background.

case appScheduled

The app scheduled this snapshot.

case complicationUpdate

The app updated the complication timeline.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

