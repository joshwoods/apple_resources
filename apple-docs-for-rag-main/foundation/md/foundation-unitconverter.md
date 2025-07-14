

- Foundation
-  UnitConverter 

Class

# UnitConverter

An abstract class that provides a description of how to convert a unit to and from the base unit of its dimension.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitConverter
```

## Overview

For units that can be converted by a scale factor or linear equation, use the concrete subclass UnitConverterLinear.

### Subclassing Notes

UnitConverter is an abstract class that is intended for subclassing. You can implement your own subclass of UnitConverter to convert between units according to any desired mapping function. For example, units may be converted using a logarithmic, exponential, or quantile scale.

#### Methods to Override

All subclasses must fully implement the following methods:

- baseUnitValue(fromValue:)

- value(fromBaseUnitValue:)

#### Alternatives to Subclassing

As stated above, most physical units can be converted using a linear equation with UnitConverterLinear. You should only create a custom subclass of UnitConverter for units that cannot be converted in this way.

## Topics

### Converting Between Units

func baseUnitValue(fromValue: Double) -> Double

For a given unit, returns the specified value of that unit in terms of the base unit of its dimension.

func value(fromBaseUnitValue: Double) -> Double

For a given unit, returns the specified value of the base unit in terms of that unit.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UnitConverterLinear

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Conversion

class UnitConverterLinear

A description of how to convert between units using a linear equation.

