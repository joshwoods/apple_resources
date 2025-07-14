

- WorkoutKit
- CadenceRangeAlert
-  cadence(\_:unit:) 

Type Method

# cadence(\_:unit:)

Creates a new cadence alert for the target range.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
static func cadence(
    _ range: ClosedRange,
    unit: UnitFrequency = WorkoutAlertMetric.countPerMinute
) -> Self
```

Available when `Self` is `CadenceRangeAlert`.

## Parameters 

`range`  

A closed range representing the cadence’s value.

`unit`  

The frequency units for the specified range.

## See Also

### Creating new cadence range alerts

init(target: ClosedRange&lt;Measurement&lt;UnitFrequency>>)

Creates a cadence alert for a closed range of measurements.

