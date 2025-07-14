

- Foundation
- Measurement
-  convert(to:) 

Instance Method

# convert(to:)

Converts the measurement to the specified unit.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
mutating func convert(to otherUnit: UnitType)
```

Available when `UnitType` inherits `Dimension`.

## Parameters 

`otherUnit`  

A unit of the same `Dimension`.

## See Also

### Converting to Other Units

func converted(to: UnitType) -> Measurement&lt;UnitType>

Returns a new measurement created by converting to the specified unit.

