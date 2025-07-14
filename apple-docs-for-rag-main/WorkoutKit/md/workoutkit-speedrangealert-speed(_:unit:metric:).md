

- WorkoutKit
- SpeedRangeAlert
-  speed(\_:unit:metric:) 

Type Method

# speed(\_:unit:metric:)

Returns a new speed alert for the provided range of values.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

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

The speed units used for the values.

`metric`  

The metric used to measure the speed.

## See Also

### Creating speed range alerts

init(target: ClosedRange&lt;Measurement&lt;UnitSpeed>>, metric: WorkoutAlertMetric)

Creates a new speed alert for the provided range of values.

