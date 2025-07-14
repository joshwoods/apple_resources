

- WorkoutKit
- CadenceRangeAlert
-  init(target:) 

Initializer

# init(target:)

Creates a cadence alert for a closed range of measurements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(target: ClosedRange>)
```

## Parameters 

`target`  

A closed range that uses frequency units.

## See Also

### Creating new cadence range alerts

static func cadence(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Creates a new cadence alert for the target range.

