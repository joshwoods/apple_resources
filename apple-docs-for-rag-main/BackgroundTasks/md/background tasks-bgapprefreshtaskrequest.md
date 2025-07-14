

- Background Tasks
-  BGAppRefreshTaskRequest 

Class

# BGAppRefreshTaskRequest

A request to launch your app in the background to execute a short refresh task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
class BGAppRefreshTaskRequest
```

## Mentioned in 

Choosing Background Strategies for Your App

## Topics

### Initializing a refresh task request

init(identifier: String)

Return a new refresh task request for the specified identifier.

## Relationships

### Inherits From

- BGTaskRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Requests

class BGProcessingTaskRequest

A request to launch your app in the background to execute a processing task that can take minutes to complete.

class BGTaskRequest

An abstract class for representing task requests.

class BGHealthResearchTaskRequest

A request to launch your app in the background to execute processing for a health research study in which a user participates.

