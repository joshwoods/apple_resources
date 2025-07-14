

- WatchKit
- WKSnapshotReason
-  WKSnapshotReason.complicationUpdate 

Case

# WKSnapshotReason.complicationUpdate

The app updated the complication timeline.

watchOS 4.0+

``` source
case complicationUpdate
```

## Discussion

These snapshot refresh tasks are only triggered when the WatchKit extension has a complication on the current watch face.

## See Also

### Enumeration Cases

case appBackgrounded

The app transitioned from the foreground to the background.

case appScheduled

The app scheduled this snapshot.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

case returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

