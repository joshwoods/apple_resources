

- WatchKit
- WKSnapshotReason
-  WKSnapshotReason.returnToDefaultState 

Case

# WKSnapshotReason.returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

watchOS 4.0+

``` source
case returnToDefaultState
```

## See Also

### Enumeration Cases

case appBackgrounded

The app transitioned from the foreground to the background.

case appScheduled

The app scheduled this snapshot.

case complicationUpdate

The app updated the complication timeline.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

