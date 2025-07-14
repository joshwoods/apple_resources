

- WatchKit
- WKSnapshotRefreshBackgroundTask
-  returnToDefaultState Deprecated

Instance Property

# returnToDefaultState

A Boolean value indicating that the app should return to its default state.

watchOS 3.0–4.0Deprecated

``` source
var returnToDefaultState: Bool { get }
```

Deprecated

Use reasonForSnapshot instead.

## See Also

### Instance properties

var reasonForSnapshot: WKSnapshotReason

The reason for taking the upcoming snapshot.

enum WKSnapshotReason

The reason for a background snapshot task.

