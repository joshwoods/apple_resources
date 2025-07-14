

- Background Tasks
- BGTaskScheduler
- BGTaskScheduler.Error
- BGTaskScheduler.Error.Code
-  BGTaskScheduler.Error.Code.notPermitted 

Case

# BGTaskScheduler.Error.Code.notPermitted

A task scheduling error indicating the app isn’t permitted to schedule the task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
case notPermitted
```

## Discussion

There are two causes for this error:

- The app doesn’t set the appropriate mode in the UIBackgroundModes array.

- The task identifier of the submitted task wasn’t in the BGTaskSchedulerPermittedIdentifiers array in the Info.plist File.

## See Also

### Enumeration cases

case tooManyPendingTaskRequests

A task scheduling error indicating that there are too many pending tasks of the type requested.

case unavailable

A task scheduling error indicating that the app or extension can’t schedule background work.

