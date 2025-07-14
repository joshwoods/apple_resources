

- HomeKit
-  HMCharacteristicValueCurrentSecuritySystemState 

Enumeration

# HMCharacteristicValueCurrentSecuritySystemState

Possible values for the current security system state.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
enum HMCharacteristicValueCurrentSecuritySystemState
```

## Topics

### Security System States

case stayArm

The home is occupied and residents are active.

case awayArm

The home is unoccupied.

case nightArm

The home is occupied and residents are sleeping.

case disarmed

The security system is disarmed.

case triggered

the security system is triggered.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

