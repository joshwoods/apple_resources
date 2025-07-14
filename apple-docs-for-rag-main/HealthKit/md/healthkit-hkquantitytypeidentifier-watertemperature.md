

- HealthKit
- HKQuantityTypeIdentifier
-  waterTemperature 

Type Property

# waterTemperature

A quantity sample that records the water temperature.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
static let waterTemperature: HKQuantityTypeIdentifier
```

## Discussion

Apple Watch Ultra automatically records these samples during dive sessions and swimming workouts.

Water temperature samples use temperature units (see HKUnit) and measure discrete values (see HKQuantityAggregationStyle).

## See Also

### Diving

static let underwaterDepth: HKQuantityTypeIdentifier

A quantity sample that records a person’s depth underwater.

