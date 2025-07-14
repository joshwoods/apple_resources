

- WatchKit
- WKRefreshBackgroundTask
-  expirationHandler 

Instance Property

# expirationHandler

A block that the system calls when the available runtime for a background task is about to expire.

watchOS 8.0+

``` source
var expirationHandler: (() -> Void)? { get set }
```

## Mentioned in 

Using background tasks

## Discussion

To respond when your background task is about to expire, assign a block to this property. In this block, clean up any running background tasks, and prepare for the system to suspend your app.

## See Also

### Completing the background task

func setTaskCompletedWithSnapshot(Bool)

Marks the task as complete and indicates whether the system should take a new snapshot of the app.

func setTaskCompleted()

Marks the task as complete.

Deprecated

