

- HomeKit
-  HMCharacteristicValueTargetHumidifierDehumidifierState 

Enumeration

# HMCharacteristicValueTargetHumidifierDehumidifierState

Possible values for the target humidifier or dehumidifier state.

iOS 10.2+iPadOS 10.2+Mac Catalyst 10.2+tvOS 10.1+visionOS 1.0+watchOS 3.1.1+

``` source
enum HMCharacteristicValueTargetHumidifierDehumidifierState
```

## Topics

### Target States

case automatic

The accessory should decide whether to add or remove water to or from the air.

case humidify

The accessory should add water to the air.

case dehumidify

The accessory should remove water from the air.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

