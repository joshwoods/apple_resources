

- HealthKit
-  HKMetadataKeyLowCardioFitnessEventThreshold 

Global Variable

# HKMetadataKeyLowCardioFitnessEventThreshold

The VO2 max threshold used to categorize low-level cardio fitness events.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 13.0+visionOS 1.0+watchOS 7.2+

``` source
let HKMetadataKeyLowCardioFitnessEventThreshold: String
```

## Discussion

The system sets this key on lowCardioFitnessEvent samples. It contains the threshold value for the user’s VO2 max measurements. The threshold value varies depending on certain parameters and physical characteristics, such as the user’s age.

A low-cardio fitness event indicates a period of time when the user’s VO2 max measurements consistently fall below the defined value. The system triggers this event approximately once every four months.

The value of this key is an HKQuantity object with a unit of `ml/(kg*min)`. For more information on working with complex units, see unitMultiplied(by:), unitDivided(by:), and init(from:).

## See Also

### Cardio Fitness Keys

let HKMetadataKeyVO2MaxValue: String

The maximum oxygen consumption rate during exercise of increasing intensity.

