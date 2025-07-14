

- WatchKit
- WKSnapshotReason
-  WKSnapshotReason.appScheduled 

Case

# WKSnapshotReason.appScheduled

The app scheduled this snapshot.

watchOS 4.0+

``` source
case appScheduled
```

## Discussion

You can schedule snapshots either by calling the scheduleSnapshotRefresh(withPreferredDate:userInfo:scheduledCompletion:) method, or—when completing a background task—by calling the setTaskCompletedWithSnapshot(_:) method and passing true.

These snapshot refresh tasks are only triggered when the watchOS app is in the dock.

## See Also

### Enumeration Cases

case appBackgrounded

The app transitioned from the foreground to the background.

case complicationUpdate

The app updated the complication timeline.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

case returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

