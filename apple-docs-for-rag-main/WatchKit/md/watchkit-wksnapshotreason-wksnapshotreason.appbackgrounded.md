

- WatchKit
- WKSnapshotReason
-  WKSnapshotReason.appBackgrounded 

Case

# WKSnapshotReason.appBackgrounded

The app transitioned from the foreground to the background.

watchOS 4.0+

``` source
case appBackgrounded
```

## See Also

### Enumeration Cases

case appScheduled

The app scheduled this snapshot.

case complicationUpdate

The app updated the complication timeline.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

case returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

