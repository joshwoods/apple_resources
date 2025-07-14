

- HealthKit
-  HKMetadataKeyWeatherTemperature 

Global Variable

# HKMetadataKeyWeatherTemperature

A key that represents the weather temperature during the sample.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
let HKMetadataKeyWeatherTemperature: String
```

## Discussion

This key takes an `HKQuantity` value expressed in a unit of temperature. Set this key on an HKWorkout object to represent the overall temperature during the workout.

## See Also

### Weather Keys

let HKMetadataKeyBarometricPressure: String

The metadata key for the barometric pressure associated with a sample.

let HKMetadataKeyWeatherCondition: String

A key that represents the weather condition during the sample.

let HKMetadataKeyWeatherHumidity: String

A key that represents the weather humidity during the sample.

