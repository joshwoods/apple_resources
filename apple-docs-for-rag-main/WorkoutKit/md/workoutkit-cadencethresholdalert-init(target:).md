

- WorkoutKit
- CadenceThresholdAlert
-  init(target:) 

Initializer

# init(target:)

Create a new cadence threshold alert for the target measurement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(target: Measurement)
```

## Parameters 

`target`  

A measurement that uses frequency units.

## See Also

### Creating new cadence threshold alerts

static func cadence(Double, unit: UnitFrequency) -> Self

Returns a new cadence threshold alert for the target value.

