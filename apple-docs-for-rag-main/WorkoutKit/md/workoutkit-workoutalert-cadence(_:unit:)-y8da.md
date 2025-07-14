

- WorkoutKit
- WorkoutAlert
-  cadence(\_:unit:) 

Type Method

# cadence(\_:unit:)

Creates a new alert for a range of cadence values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

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

### Creating cadence alerts

struct CadenceRangeAlert

An alert for a range of cadence values.

static func cadence(Double, unit: UnitFrequency) -> Self

Creates an alert for the specified cadence threshold.

struct CadenceThresholdAlert

An alert for a cadence threshold.

