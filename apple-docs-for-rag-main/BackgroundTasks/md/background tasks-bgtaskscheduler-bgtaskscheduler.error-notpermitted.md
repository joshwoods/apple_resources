

- Background Tasks
- BGTaskScheduler
- BGTaskScheduler.Error
-  notPermitted 

Type Property

# notPermitted

A task scheduling error indicating the app isn’t permitted to launch the task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
static var notPermitted: BGTaskScheduler.Error.Code { get }
```

## Discussion

There are two causes for this error:

- The app doesn’t set the appropriate mode in the UIBackgroundModes array.

- The task identifier of the submitted task wasn’t in the BGTaskSchedulerPermittedIdentifiers array in The Info.plist File.

## See Also

### Getting the error codes

enum Code

An enumeration of the task scheduling errors.

static var tooManyPendingTaskRequests: BGTaskScheduler.Error.Code

A task scheduling error indicating that there are too many pending tasks of the type requested.

static var unavailable: BGTaskScheduler.Error.Code

A task scheduling error indicating that the app or extension can’t schedule background work.

