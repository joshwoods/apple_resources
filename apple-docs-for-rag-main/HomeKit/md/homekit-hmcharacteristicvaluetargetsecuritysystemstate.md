

- HomeKit
-  HMCharacteristicValueTargetSecuritySystemState 

Enumeration

# HMCharacteristicValueTargetSecuritySystemState

Possible values for the target security system state.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
enum HMCharacteristicValueTargetSecuritySystemState
```

## Topics

### Security System States

case stayArm

The home is occupied and residents are active.

case awayArm

The home is unoccupied.

case nightArm

The home is occupied and residents are sleeping.

case disarm

The security system is disarmed.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

