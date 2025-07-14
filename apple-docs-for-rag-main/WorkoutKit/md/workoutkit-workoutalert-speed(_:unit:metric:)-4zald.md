

- WorkoutKit
- WorkoutAlert
-  speed(\_:unit:metric:) 

Type Method

# speed(\_:unit:metric:)

Creates a new speed threshold alert.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func speed(
    _ value: Double,
    unit: UnitSpeed,
    metric: WorkoutAlertMetric = .current
) -> Self
```

Available when `Self` is `SpeedThresholdAlert`.

## Parameters 

`value`  

The threshold value.

`unit`  

The speed units used by the threshold value.

`metric`  

The metric used to measure the speed.

## See Also

### Creating speed alerts

static func speed(ClosedRange&lt;Double>, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Creates a new speed alert for the provided range.

struct SpeedRangeAlert

An alert for a range of speed values.

struct SpeedThresholdAlert

An alert for a speed threshold.

