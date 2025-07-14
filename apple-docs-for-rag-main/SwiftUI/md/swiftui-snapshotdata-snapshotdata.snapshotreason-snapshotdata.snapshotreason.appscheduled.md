

- SwiftUI
- SnapshotData
- SnapshotData.SnapshotReason
-  SnapshotData.SnapshotReason.appScheduled 

Case

# SnapshotData.SnapshotReason.appScheduled

The app scheduled this snapshot.

watchOS 9.0+

``` source
case appScheduled
```

## See Also

### Getting the snapshot reasons

case appBackgrounded

The app transitioned from the foreground to the background.

case complicationUpdate

The app updated the complication timeline.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

case returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

