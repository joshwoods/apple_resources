

- WorkoutKit
- HeartRateRangeAlert
-  heartRate(\_:unit:) 

Type Method

# heartRate(\_:unit:)

Returns a new heart rate alert for the target range.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
static func heartRate(
    _ range: ClosedRange,
    unit: UnitFrequency = WorkoutAlertMetric.countPerMinute
) -> Self
```

Available when `Self` is `HeartRateRangeAlert`.

## Parameters 

`range`  

A closed range of heart rate values.

`unit`  

The frequency units used by the range values.

## See Also

### Creating new heart rate alerts

init(target: ClosedRange&lt;Measurement&lt;UnitFrequency>>)

Creates a new heart rate alert for a closed range of measurements.

