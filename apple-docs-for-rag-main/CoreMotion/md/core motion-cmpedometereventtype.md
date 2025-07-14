

- Core Motion
-  CMPedometerEventType 

Enumeration

# CMPedometerEventType

Constants indicating the change that occurred to the user’s pedestrian activity.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 3.0+

``` source
enum CMPedometerEventType
```

## Topics

### Enumeration Cases

case pause

The user’s pedestrian activity stopped.

case resume

The user’s pedestrian activity resumed.

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

### Pedometer Data

var date: Date

The date on which the pedometer event was recorded.

var type: CMPedometerEventType

The type of change that occurred.

