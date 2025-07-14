

- Background Tasks
- BGTaskScheduler
- BGTaskScheduler.Error
-  BGTaskScheduler.Error.Code 

Enumeration

# BGTaskScheduler.Error.Code

An enumeration of the task scheduling errors.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Enumeration cases

case notPermitted

A task scheduling error indicating the app isn’t permitted to schedule the task.

case tooManyPendingTaskRequests

A task scheduling error indicating that there are too many pending tasks of the type requested.

case unavailable

A task scheduling error indicating that the app or extension can’t schedule background work.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling errors

struct Error

The Errors for the `BGTaskSchedulerError` domain.

class let errorDomain: String

The background tasks error domain as a string.

