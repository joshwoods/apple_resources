

- WorkoutKit
- HeartRateRangeAlert
-  init(target:) 

Initializer

# init(target:)

Creates a new heart rate alert for a closed range of measurements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(target: ClosedRange>)
```

## Parameters 

`target`  

A range of values that use frequency units.

## See Also

### Creating new heart rate alerts

static func heartRate(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Returns a new heart rate alert for the target range.

