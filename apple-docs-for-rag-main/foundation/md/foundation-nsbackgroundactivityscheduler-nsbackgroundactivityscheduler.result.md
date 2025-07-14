

- Foundation
- NSBackgroundActivityScheduler
-  NSBackgroundActivityScheduler.Result 

Enumeration

# NSBackgroundActivityScheduler.Result

These constants indicate whether background activity has been completed successfully or whether additional processing should be deferred until a more optimal time.

macOS 10.10+

``` source
enum Result
```

## Topics

### Constants

case finished

The activity has finished executing. If the activity repeats, the next invocation is scheduled by the system.

case deferred

System conditions have changed since the time the activity began executing, and deferral of additional work is recommended.

case finished

The activity has finished executing. If the activity repeats, the next invocation is scheduled by the system.

case deferred

System conditions have changed since the time the activity began executing, and deferral of additional work is recommended.

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

### Constants

enum QualityOfService

Constants that indicate the nature and importance of work to the system.

