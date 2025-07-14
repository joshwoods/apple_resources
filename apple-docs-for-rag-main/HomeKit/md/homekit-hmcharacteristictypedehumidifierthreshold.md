

- HomeKit
-  HMCharacteristicTypeDehumidifierThreshold 

Global Variable

# HMCharacteristicTypeDehumidifierThreshold

The humidity above which a dehumidifier should begin to work.

iOS 10.2+iPadOS 10.2+Mac Catalyst 10.2+tvOS 10.1+visionOS 1.0+watchOS 3.1.1+

``` source
let HMCharacteristicTypeDehumidifierThreshold: String
```

## Discussion

The corresponding value is a floating point percentage representing the relative humidity threshold. Relative humidity is a measure of the amount of water in the air relative to the maximum it can hold at the current temperature.

## See Also

### Humidity

let HMCharacteristicTypeCurrentRelativeHumidity: String

The current relative humidity measured by the accessory.

let HMCharacteristicTypeTargetRelativeHumidity: String

The target relative humidity for the accessory to achieve.

let HMCharacteristicTypeCurrentHumidifierDehumidifierState: String

The current state of a humidifier or dehumidifier accessory.

let HMCharacteristicTypeTargetHumidifierDehumidifierState: String

The state that a humidifier or dehumidifier accessory should try to achieve.

let HMCharacteristicTypeHumidifierThreshold: String

The humidity below which a humidifier should begin to work.

