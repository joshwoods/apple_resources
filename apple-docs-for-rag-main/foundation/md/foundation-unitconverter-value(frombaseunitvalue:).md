

- Foundation
- UnitConverter
-  value(fromBaseUnitValue:) 

Instance Method

# value(fromBaseUnitValue:)

For a given unit, returns the specified value of the base unit in terms of that unit.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func value(fromBaseUnitValue baseUnitValue: Double) -> Double
```

## Parameters 

`baseUnitValue`  

The value in terms of the base unit.

## Return Value

The value in terms of a given unit.

## Discussion

This method takes a value in the base unit of a unit’s dimension and returns the result of converting it into that unit. For example, a converter for the pounds unit calling this method, passing `2.20462` to the `baseUnitValue` parameter, results in `1.0` (*2.20462 lbs = 1 kg*).

## See Also

### Converting Between Units

func baseUnitValue(fromValue: Double) -> Double

For a given unit, returns the specified value of that unit in terms of the base unit of its dimension.

