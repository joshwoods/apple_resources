

- Foundation
- Measurement
-  converted(to:) 

Instance Method

# converted(to:)

Returns a new measurement created by converting to the specified unit.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func converted(to otherUnit: UnitType) -> Measurement
```

Available when `UnitType` inherits `Dimension`.

## Parameters 

`otherUnit`  

A unit of the same `Dimension`.

## Return Value

A converted measurement.

## See Also

### Converting to Other Units

func convert(to: UnitType)

Converts the measurement to the specified unit.

