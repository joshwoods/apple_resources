

- WorkoutKit
- PowerRangeAlert
-  power(\_:unit:) 

Type Method

# power(\_:unit:)

Returns a new power alert for the target range.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
static func power(
    _ range: ClosedRange,
    unit: UnitPower
) -> Self
```

Available when `Self` is `PowerRangeAlert`.

## Parameters 

`range`  

A closed range of power values.

`unit`  

The power units used by the range values.

## See Also

### Creating new power range alerts

init(target: ClosedRange&lt;Measurement&lt;UnitPower>>)

Creates a new power alert for the target range.

