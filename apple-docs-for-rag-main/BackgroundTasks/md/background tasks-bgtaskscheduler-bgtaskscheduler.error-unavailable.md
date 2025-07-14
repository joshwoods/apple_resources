

- Background Tasks
- BGTaskScheduler
- BGTaskScheduler.Error
-  unavailable 

Type Property

# unavailable

A task scheduling error indicating that the app or extension can’t schedule background work.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
static var unavailable: BGTaskScheduler.Error.Code { get }
```

## Discussion

This error usually occurs for one of three reasons:

- The user has disabled background refresh in settings.

- The app is running on Simulator which doesn’t support background processing.

- The extension either hasn’t set RequestsOpenAccess to `YES` in The Info.plist File, or the user hasn’t granted open access.

## See Also

### Getting the error codes

enum Code

An enumeration of the task scheduling errors.

static var notPermitted: BGTaskScheduler.Error.Code

A task scheduling error indicating the app isn’t permitted to launch the task.

static var tooManyPendingTaskRequests: BGTaskScheduler.Error.Code

A task scheduling error indicating that there are too many pending tasks of the type requested.

