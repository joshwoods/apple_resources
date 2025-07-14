

- WorkoutKit
- PowerThresholdAlert
-  power(\_:unit:) 

Type Method

# power(\_:unit:)

Returns a new power threshold alert for the target value.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
static func power(
    _ value: Double,
    unit: UnitPower
) -> Self
```

Available when `Self` is `PowerThresholdAlert`.

## Parameters 

`value`  

The target value of the power threshold.

`unit`  

The power units used by the target value.

## See Also

### Creating power threshold alerts

init(target: Measurement&lt;UnitPower>)

Returns a new power threshold alert for the target measurement.

