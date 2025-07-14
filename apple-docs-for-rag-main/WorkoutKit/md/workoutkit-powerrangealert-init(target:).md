

- WorkoutKit
- PowerRangeAlert
-  init(target:) 

Initializer

# init(target:)

Creates a new power alert for the target range.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(target: ClosedRange>)
```

## Parameters 

`target`  

A closed range of measurement values using power units.

## See Also

### Creating new power range alerts

static func power(ClosedRange&lt;Double>, unit: UnitPower) -> Self

Returns a new power alert for the target range.

