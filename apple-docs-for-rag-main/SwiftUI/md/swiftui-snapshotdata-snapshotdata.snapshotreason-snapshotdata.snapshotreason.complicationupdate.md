

- SwiftUI
- SnapshotData
- SnapshotData.SnapshotReason
-  SnapshotData.SnapshotReason.complicationUpdate 

Case

# SnapshotData.SnapshotReason.complicationUpdate

The app updated the complication timeline.

watchOS 9.0+

``` source
case complicationUpdate
```

## See Also

### Getting the snapshot reasons

case appBackgrounded

The app transitioned from the foreground to the background.

case appScheduled

The app scheduled this snapshot.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

case returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

