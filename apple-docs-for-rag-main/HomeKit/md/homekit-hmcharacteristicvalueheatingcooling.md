

- HomeKit
-  HMCharacteristicValueHeatingCooling 

Enumeration

# HMCharacteristicValueHeatingCooling

Possible values for the heating or cooling characteristic of a thermostat.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
enum HMCharacteristicValueHeatingCooling
```

## Topics

### Accesory State

case off

Unit is set to off, neither heating nor cooling.

case heat

Unit is set to heating.

case cool

Unit is set to cooling.

case auto

Unit is set to automatic.

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

### Values

enum HMCharacteristicValueCurrentHeatingCooling

States that indicate an accessory’s process of increasing or decreasing temperature.

