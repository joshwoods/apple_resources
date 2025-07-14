

- HomeKit
-  HMCharacteristicValueDoorState 

Enumeration

# HMCharacteristicValueDoorState

Possible values for the state of a door.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
enum HMCharacteristicValueDoorState
```

## Topics

### Door States

case open

The door is fully open.

case closed

The door is fully closed.

case opening

The door is actively opening.

case closing

The door is actively closing.

case stopped

The door is not moving, and is neither fully open nor fully closed.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

