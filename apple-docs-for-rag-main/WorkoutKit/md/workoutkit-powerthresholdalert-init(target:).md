

- WorkoutKit
- PowerThresholdAlert
-  init(target:) 

Initializer

# init(target:)

Returns a new power threshold alert for the target measurement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(target: Measurement)
```

## Parameters 

`target`  

A measurement that uses power units.

## See Also

### Creating power threshold alerts

static func power(Double, unit: UnitPower) -> Self

Returns a new power threshold alert for the target value.

