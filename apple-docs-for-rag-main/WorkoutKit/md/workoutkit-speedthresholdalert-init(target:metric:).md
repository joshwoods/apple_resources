

- WorkoutKit
- SpeedThresholdAlert
-  init(target:metric:) 

Initializer

# init(target:metric:)

Creates a new speed threshold alert.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(
    target: Measurement,
    metric: WorkoutAlertMetric
)
```

## Parameters 

`target`  

A speed measurement that represents the target threshold.

`metric`  

The metric used to measure the speed.

## See Also

### Creating speed threshold alerts

static func speed(Double, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Returns a new speed threshold alert.

