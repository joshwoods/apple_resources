

- HealthKit
-  HKMetadataKeyWeatherCondition 

Global Variable

# HKMetadataKeyWeatherCondition

A key that represents the weather condition during the sample.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
let HKMetadataKeyWeatherCondition: String
```

## Discussion

This key takes an an NSNumber value that contains an HKWeatherCondition value. Set this key on an HKWorkout object to represent the overall weather condition during the workout.

## Topics

### Valid Weather Conditions

enum HKWeatherCondition

Constants that indicate a type of weather.

## See Also

### Weather Keys

let HKMetadataKeyBarometricPressure: String

The metadata key for the barometric pressure associated with a sample.

let HKMetadataKeyWeatherHumidity: String

A key that represents the weather humidity during the sample.

let HKMetadataKeyWeatherTemperature: String

A key that represents the weather temperature during the sample.

