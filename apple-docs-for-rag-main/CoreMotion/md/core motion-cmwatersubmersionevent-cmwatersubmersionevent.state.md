

- Core Motion
- CMWaterSubmersionEvent
-  CMWaterSubmersionEvent.State 

Enumeration

# CMWaterSubmersionEvent.State

The device’s submersion state.

iOS 4.0+iPadOS 4.0+visionOS 1.0+watchOS 2.0+

``` source
enum State
```

## Topics

### Submersion states

case notSubmerged

The device isn’t submerged in water.

case submerged

The device is submerged in water.

case unknown

The submersion state is unknown.

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

### Accessing event data

var date: Date

The time and date of the event.

var state: CMWaterSubmersionEvent.State

The new submersion state.

