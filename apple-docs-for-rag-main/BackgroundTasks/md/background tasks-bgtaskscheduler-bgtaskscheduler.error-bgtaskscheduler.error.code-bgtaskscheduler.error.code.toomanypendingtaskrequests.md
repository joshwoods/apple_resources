

- Background Tasks
- BGTaskScheduler
- BGTaskScheduler.Error
- BGTaskScheduler.Error.Code
-  BGTaskScheduler.Error.Code.tooManyPendingTaskRequests 

Case

# BGTaskScheduler.Error.Code.tooManyPendingTaskRequests

A task scheduling error indicating that there are too many pending tasks of the type requested.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
case tooManyPendingTaskRequests
```

## Discussion

Try canceling some existing task requests and then resubmit the request that failed.

## See Also

### Enumeration cases

case notPermitted

A task scheduling error indicating the app isn’t permitted to schedule the task.

case unavailable

A task scheduling error indicating that the app or extension can’t schedule background work.

