

- HomeKit
-  HMCharacteristicTypeTemperatureUnits 

Global Variable

# HMCharacteristicTypeTemperatureUnits

The units of temperature currently active on the accessory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
let HMCharacteristicTypeTemperatureUnits: String
```

## Discussion

The corresponding value is one of the constants from the HMCharacteristicValueTemperatureUnit enumeration.

HomeKit always reports temperature values in degrees Celsius, but your app should display the temperature in units chosen by the user.

## Topics

### Values

enum HMCharacteristicValueTemperatureUnit

Possible values for the temperature units currently active on the accessory.

## See Also

### Temperature

let HMCharacteristicTypeCurrentTemperature: String

The current temperature measured by the accessory.

let HMCharacteristicTypeTargetTemperature: String

The target temperature for the accessory to achieve.

let HMCharacteristicTypeTargetHeatingCooling: String

The target heating or cooling mode for a thermostat.

let HMCharacteristicTypeCurrentHeatingCooling: String

The current heating or cooling mode for a thermostat.

let HMCharacteristicTypeTargetHeaterCoolerState: String

The target state for a device that heats or cools, like an oven or a refrigerator.

let HMCharacteristicTypeCurrentHeaterCoolerState: String

The current state for a device that heats or cools, like an oven or a refrigerator.

let HMCharacteristicTypeCoolingThreshold: String

The temperature above which cooling will be active.

let HMCharacteristicTypeHeatingThreshold: String

The temperature below which heating will be active.

