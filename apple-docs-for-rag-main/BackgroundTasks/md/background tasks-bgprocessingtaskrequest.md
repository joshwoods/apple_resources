

- Background Tasks
-  BGProcessingTaskRequest 

Class

# BGProcessingTaskRequest

A request to launch your app in the background to execute a processing task that can take minutes to complete.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
class BGProcessingTaskRequest
```

## Topics

### Initializing a Processing Task Request

init(identifier: String)

Return a new processing task request for the specified identifier.

### Setting Task Request Options

var requiresExternalPower: Bool

A Boolean specifying if the processing task requires a device connected to power.

var requiresNetworkConnectivity: Bool

A Boolean specifying if the processing task requires network connectivity.

## Relationships

### Inherits From

- BGTaskRequest

### Inherited By

- BGHealthResearchTaskRequest

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

class BGAppRefreshTaskRequest

A request to launch your app in the background to execute a short refresh task.

class BGTaskRequest

An abstract class for representing task requests.

class BGHealthResearchTaskRequest

A request to launch your app in the background to execute processing for a health research study in which a user participates.

