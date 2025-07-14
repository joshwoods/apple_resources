

- HomeKit
-  HMCharacteristicValueLockMechanismState 

Enumeration

# HMCharacteristicValueLockMechanismState

Possible values for the state of a lock mechanism.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
enum HMCharacteristicValueLockMechanismState
```

## Topics

### Lock Mechanism State

case unsecured

The lock mechanism is unlocked.

case secured

The lock mechanism is locked.

case jammed

The lock mechanism is jammed.

case unknown

The lock mechanism is in an unknown state.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

