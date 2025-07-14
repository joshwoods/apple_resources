

- WatchKit
- WKSnapshotRefreshBackgroundTask
-  reasonForSnapshot 

Instance Property

# reasonForSnapshot

The reason for taking the upcoming snapshot.

watchOS 4.0+

``` source
var reasonForSnapshot: WKSnapshotReason { get }
```

## Discussion

You can use this property to change your application’s appearance before a snapshot is taken. For example, if the property contains an WKSnapshotReason.appBackgrounded value, you’d probably want to capture the app’s current state, and no changes are necessary. However, if the property contains a WKSnapshotReason.returnToDefaultState value, you may want to navigate back to the root view controller before taking the snapshot.

For a list of possible reasons for taking the snapshot, see WKSnapshotReason.

## See Also

### Instance properties

enum WKSnapshotReason

The reason for a background snapshot task.

var returnToDefaultState: Bool

A Boolean value indicating that the app should return to its default state.

Deprecated

