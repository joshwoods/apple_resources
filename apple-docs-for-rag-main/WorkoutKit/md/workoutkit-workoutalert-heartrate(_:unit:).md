

- WorkoutKit
- WorkoutAlert
-  heartRate(\_:unit:) 

Type Method

# heartRate(\_:unit:)

Creates a new heart rate alert for the target range.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

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

### Creating heart rate alerts

struct HeartRateRangeAlert

An alert for a range of heart rates.

static func heartRate(zone: Int) -> Self

Creates a new alert for the specified heart rate zone.

struct HeartRateZoneAlert

An alert for a heart rate zone.

