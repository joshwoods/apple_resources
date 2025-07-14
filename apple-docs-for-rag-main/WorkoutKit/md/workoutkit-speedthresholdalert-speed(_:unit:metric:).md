

- WorkoutKit
- SpeedThresholdAlert
-  speed(\_:unit:metric:) 

Type Method

# speed(\_:unit:metric:)

Returns a new speed threshold alert.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

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

The value of the target threshold.

`unit`  

The speed units used by the value.

`metric`  

The metric used to measure the speed.

## See Also

### Creating speed threshold alerts

init(target: Measurement&lt;UnitSpeed>, metric: WorkoutAlertMetric)

Creates a new speed threshold alert.

