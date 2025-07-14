

- HomeKit
-  HMCharacteristicValueCurrentHeatingCooling 

Enumeration

# HMCharacteristicValueCurrentHeatingCooling

States that indicate an accessory’s process of increasing or decreasing temperature.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
enum HMCharacteristicValueCurrentHeatingCooling
```

## Topics

### Temperature States

case cool

The accessory state indicates cooling.

case heat

The accessory state indicates heating.

case off

The accessory indicates no heating or cooling.

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

enum HMCharacteristicValueHeatingCooling

Possible values for the heating or cooling characteristic of a thermostat.

