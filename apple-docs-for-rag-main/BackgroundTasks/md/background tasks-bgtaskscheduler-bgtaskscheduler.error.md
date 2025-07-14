

- Background Tasks
- BGTaskScheduler
-  BGTaskScheduler.Error 

Structure

# BGTaskScheduler.Error

The Errors for the `BGTaskSchedulerError` domain.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
struct Error
```

## Topics

### Getting the error codes

enum Code

An enumeration of the task scheduling errors.

static var notPermitted: BGTaskScheduler.Error.Code

A task scheduling error indicating the app isn’t permitted to launch the task.

static var tooManyPendingTaskRequests: BGTaskScheduler.Error.Code

A task scheduling error indicating that there are too many pending tasks of the type requested.

static var unavailable: BGTaskScheduler.Error.Code

A task scheduling error indicating that the app or extension can’t schedule background work.

### Getting the error domain

static var errorDomain: String

The background tasks error domain as a string.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Handling errors

enum Code

An enumeration of the task scheduling errors.

class let errorDomain: String

The background tasks error domain as a string.

