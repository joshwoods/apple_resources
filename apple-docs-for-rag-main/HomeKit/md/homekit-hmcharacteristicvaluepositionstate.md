

- HomeKit
-  HMCharacteristicValuePositionState 

Enumeration

# HMCharacteristicValuePositionState

Possible values for the position states of an accessory like a door, window, awning, or window covering.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
enum HMCharacteristicValuePositionState
```

## Topics

### Position States

case closing

The position is moving towards minimum value.

case opening

The position is moving towards maximum value.

case stopped

The accessory isn’t moving.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

