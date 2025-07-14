

- HomeKit
-  HMCharacteristicValueCurrentHumidifierDehumidifierState 

Enumeration

# HMCharacteristicValueCurrentHumidifierDehumidifierState

Possible values for the current humidifier or dehumidifier state.

iOS 10.2+iPadOS 10.2+Mac Catalyst 10.2+tvOS 10.1+visionOS 1.0+watchOS 3.1.1+

``` source
enum HMCharacteristicValueCurrentHumidifierDehumidifierState
```

## Topics

### Current States

case inactive

The accesory is off.

case idle

The accessory is idle.

case humidifying

The accessory is adding water to the air.

case dehumidifying

The accessory is removing water from the air.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

