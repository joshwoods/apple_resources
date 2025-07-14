

- WatchKit
- WKRefreshBackgroundTask
-  setTaskCompletedWithSnapshot(\_:) 

Instance Method

# setTaskCompletedWithSnapshot(\_:)

Marks the task as complete and indicates whether the system should take a new snapshot of the app.

watchOS 4.0+

``` source
func setTaskCompletedWithSnapshot(_ refreshSnapshot: Bool)
```

## Parameters 

`refreshSnapshot`  

A Boolean value that indicates whether the system should take a new snapshot of the app.

## Mentioned in 

Using background tasks

Preparing to take your watchOS app’s snapshot

## Discussion

Call this method as soon as a nonsnapshot background task (any WKRefreshBackgroundTask subclass except the WKSnapshotRefreshBackgroundTask class) is complete.

To update the app’s snapshot in response to the current task, pass true, and the system schedules an immediate snapshot. This request counts against the standard snapshot budget and overwrites any requests made using the scheduleSnapshotRefresh(withPreferredDate:userInfo:scheduledCompletion:) method. As with all snapshots, your app receives a WKSnapshotRefreshBackgroundTask before the snapshot is taken.

The system provides your extension with a limited amount of time (on the order of seconds) to finish this task. If you do not call setTaskCompletedWithSnapshot(_:) on the task, the system continues to run in the background until all available time is consumed, wasting battery power.

The system suspends the extension as soon as all background tasks are complete.

When completing a snapshot background task, you generally call the setTaskCompleted(restoredDefaultState:estimatedSnapshotExpiration:userInfo:)method and explicitly set the date for the next snapshot. You can call setTaskCompletedWithSnapshot(_:) as a simpler alternative. If you pass true, the system schedules a new snapshot task in one hour. If you pass false, no snapshot is scheduled.

## See Also

### Completing the background task

var expirationHandler: (() -> Void)?

A block that the system calls when the available runtime for a background task is about to expire.

func setTaskCompleted()

Marks the task as complete.

Deprecated

