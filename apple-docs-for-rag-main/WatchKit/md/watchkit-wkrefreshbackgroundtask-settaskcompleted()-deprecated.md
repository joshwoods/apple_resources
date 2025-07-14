

- WatchKit
- WKRefreshBackgroundTask
-  setTaskCompleted() Deprecated

Instance Method

# setTaskCompleted()

Marks the task as complete.

watchOS 3.0–4.0Deprecated

``` source
func setTaskCompleted()
```

Deprecated

Use setTaskCompletedWithSnapshot(_:) instead.

## Discussion

Call this method as soon as you have finished the background task. The system provides your extension with a limited amount of time to finish the task (on the order of seconds). If you do not call setTaskCompleted() on the task, the system continues to run in the background until all the available time is consumed, wasting battery power.

The system suspends the extension as soon as all background tasks are complete.

## See Also

### Completing the background task

var expirationHandler: (() -> Void)?

A block that the system calls when the available runtime for a background task is about to expire.

func setTaskCompletedWithSnapshot(Bool)

Marks the task as complete and indicates whether the system should take a new snapshot of the app.

