

- Background Tasks
- BGTaskScheduler
- BGTaskScheduler.Error
-  tooManyPendingTaskRequests 

Type Property

# tooManyPendingTaskRequests

A task scheduling error indicating that there are too many pending tasks of the type requested.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
static var tooManyPendingTaskRequests: BGTaskScheduler.Error.Code { get }
```

## Discussion

Try canceling some existing task requests and then resubmit the request that failed.

## See Also

### Getting the error codes

enum Code

An enumeration of the task scheduling errors.

static var notPermitted: BGTaskScheduler.Error.Code

A task scheduling error indicating the app isn’t permitted to launch the task.

static var unavailable: BGTaskScheduler.Error.Code

A task scheduling error indicating that the app or extension can’t schedule background work.

