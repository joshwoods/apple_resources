

- HealthKit
-  HKMetadataKeyVO2MaxValue 

Global Variable

# HKMetadataKeyVO2MaxValue

The maximum oxygen consumption rate during exercise of increasing intensity.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 13.0+visionOS 1.0+watchOS 7.2+

``` source
let HKMetadataKeyVO2MaxValue: String
```

## Discussion

The system sets this key on lowCardioFitnessEvent samples. It contains the value of the VO2 max measurement that triggered the event. The value of this key is an HKQuantity object with a unit of `ml/(kg*min)`. For more information on working with complex units, see unitMultiplied(by:), unitDivided(by:), and init(from:).

## See Also

### Cardio Fitness Keys

let HKMetadataKeyLowCardioFitnessEventThreshold: String

The VO2 max threshold used to categorize low-level cardio fitness events.

