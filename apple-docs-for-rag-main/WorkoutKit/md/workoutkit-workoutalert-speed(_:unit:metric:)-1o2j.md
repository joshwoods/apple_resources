

- WorkoutKit
- WorkoutAlert
-  speed(\_:unit:metric:) 

Type Method

# speed(\_:unit:metric:)

Creates a new speed alert for the provided range.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func speed(
    _ range: ClosedRange,
    unit: UnitSpeed,
    metric: WorkoutAlertMetric = .current
) -> Self
```

Available when `Self` is `SpeedRangeAlert`.

## Parameters 

`range`  

A closed range of speed values.

`unit`  

The speed units used by the range.

`metric`  

The metric used for the speed measurements.

## See Also

### Creating speed alerts

struct SpeedRangeAlert

An alert for a range of speed values.

static func speed(Double, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Creates a new speed threshold alert.

struct SpeedThresholdAlert

An alert for a speed threshold.

