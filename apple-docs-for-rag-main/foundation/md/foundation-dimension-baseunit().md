

- Foundation
- Dimension
-  baseUnit() 

Type Method

# baseUnit()

Returns the base unit.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func baseUnit() -> Self
```

## Return Value

An `NSDimension` subclass object from which all other units provided by the subclass are defined.

## Discussion

The default implementation returns `nil` to indicate that the `NSDimension` class should not be used directly.

When implementing a subclass, you should return a unit converter that returns the inputted value for both the `baseUnitValueFromValue:` and `valueFromBaseUnitValue:` methods. You can create a unit converter for a base unit using the UnitConverterLinear init(coefficient:) initializer, passing `1` as the coefficient.

