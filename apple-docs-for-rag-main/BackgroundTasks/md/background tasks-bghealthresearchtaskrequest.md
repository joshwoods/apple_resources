

- Background Tasks
-  BGHealthResearchTaskRequest 

Class

# BGHealthResearchTaskRequest

A request to launch your app in the background to execute processing for a health research study in which a user participates.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
class BGHealthResearchTaskRequest
```

## Mentioned in 

Choosing Background Strategies for Your App

## Topics

### Setting file permissions

var protectionTypeOfRequiredData: NSString

The file protection required to access health research data relevant to complete the task.

## Relationships

### Inherits From

- BGProcessingTaskRequest

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

class BGAppRefreshTaskRequest

A request to launch your app in the background to execute a short refresh task.

class BGTaskRequest

An abstract class for representing task requests.

