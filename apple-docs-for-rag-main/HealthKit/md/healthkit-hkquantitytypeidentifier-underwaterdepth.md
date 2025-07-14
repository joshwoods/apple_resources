

- HealthKit
- HKQuantityTypeIdentifier
-  underwaterDepth 

Type Property

# underwaterDepth

A quantity sample that records a person’s depth underwater.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
static let underwaterDepth: HKQuantityTypeIdentifier
```

## Discussion

Apple Watch Ultra automatically records these samples during dive sessions.

Underwater depth samples use length units (described in HKUnit) and measure discrete values (described in HKQuantityAggregationStyle).

## See Also

### Diving

static let waterTemperature: HKQuantityTypeIdentifier

A quantity sample that records the water temperature.

