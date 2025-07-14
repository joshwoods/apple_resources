

- Background Tasks
-  BGTask 

Class

# BGTask

An abstract class representing a task that’s run while the app is in the background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
class BGTask
```

## Topics

### Reading Task Information

var identifier: String

The string identifier of the task.

### Configuring a Task

var expirationHandler: (() -> Void)?

A handler called shortly before the task’s background time expires.

func setTaskCompleted(success: Bool)

Informs the background task scheduler that the task is complete.

## Relationships

### Inherits From

- NSObject

### Inherited By

- BGAppRefreshTask
- BGProcessingTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Task management

class BGProcessingTask

A time-consuming processing task that runs while the app is in the background.

class BGAppRefreshTask

An object representing a short task typically used to refresh content that’s run while the app is in the background.

class BGHealthResearchTask

A time-consuming, necessary processing task that runs while the app is in the background to prepare data essential to a health research study.

