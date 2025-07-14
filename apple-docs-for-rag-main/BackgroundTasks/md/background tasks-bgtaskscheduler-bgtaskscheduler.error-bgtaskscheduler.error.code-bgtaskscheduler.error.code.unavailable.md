

- Background Tasks
- BGTaskScheduler
- BGTaskScheduler.Error
- BGTaskScheduler.Error.Code
-  BGTaskScheduler.Error.Code.unavailable 

Case

# BGTaskScheduler.Error.Code.unavailable

A task scheduling error indicating that the app or extension can’t schedule background work.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
case unavailable
```

## Discussion

This error usually occurs for one of following reasons:

- The user has disabled background refresh in settings.

- The app is running on Simulator which doesn’t support background processing.

- The keyboard extension either hasn’t set RequestsOpenAccess to `YES` in The Info.plist File, or the user hasn’t granted open access.

- The extension type isn’t able to schedule background tasks.

## See Also

### Enumeration cases

case notPermitted

A task scheduling error indicating the app isn’t permitted to schedule the task.

case tooManyPendingTaskRequests

A task scheduling error indicating that there are too many pending tasks of the type requested.

