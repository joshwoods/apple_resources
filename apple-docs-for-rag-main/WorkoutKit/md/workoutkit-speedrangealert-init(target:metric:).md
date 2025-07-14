

- WorkoutKit
- SpeedRangeAlert
-  init(target:metric:) 

Initializer

# init(target:metric:)

Creates a new speed alert for the provided range of values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(
    target: ClosedRange>,
    metric: WorkoutAlertMetric
)
```

## Parameters 

`target`  

A range of speed measurements.

`metric`  

The metric used to measure the speed.

## See Also

### Creating speed range alerts

static func speed(ClosedRange&lt;Double>, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Returns a new speed alert for the provided range of values.

