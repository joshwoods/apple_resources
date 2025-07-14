

- WorkoutKit
- CadenceThresholdAlert
-  cadence(\_:unit:) 

Type Method

# cadence(\_:unit:)

Returns a new cadence threshold alert for the target value.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
static func cadence(
    _ value: Double,
    unit: UnitFrequency = WorkoutAlertMetric.countPerMinute
) -> Self
```

Available when `Self` is `CadenceThresholdAlert`.

## Parameters 

`value`  

The threshold’s value.

`unit`  

The frequency units used by the threshold’s value.

## See Also

### Creating new cadence threshold alerts

init(target: Measurement&lt;UnitFrequency>)

Create a new cadence threshold alert for the target measurement.

