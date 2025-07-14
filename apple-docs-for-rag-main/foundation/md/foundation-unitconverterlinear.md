

- Foundation
-  UnitConverterLinear 

Class

# UnitConverterLinear

A description of how to convert between units using a linear equation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitConverterLinear
```

## Overview

A linear equation for unit conversion takes the form `y = mx + b`, such that the following is true:

- `y` is the value in terms of the base unit of the dimension.

- `m` is the known coefficient to use for this unit’s conversion.

- `x` is the value in terms of the unit on which you call this method.

- `b` is the known constant to use for this unit’s conversion.

The `baseUnitValueFromValue:` method performs the conversion in the form of `y = mx + b`, where `x` represents the value passed in and `y` represents the value returned. The `valueFromBaseUnitValue:` method performs the inverse conversion in the form of `x = (y - b) / m`, where `y` represents the value passed in and `x` represents the value returned.

For example, consider the fahrenheit unit that UnitTemperature defines. The baseUnitValue(fromValue:) method calculates the value in the base unit, kelvin, using the formula `K = (0.55555555555556) × °F + 255.37222222222427`. The value(fromBaseUnitValue:) method calculates the value in fahrenheit using the formula `°F = (K — 255.37222222222427) / (0.55555555555556)`, where the coefficient is `(0.55555555555556)` and the constant is `255.37222222222427`.

- Swift
- Objective-C

```
let kelvinToFahrenheit = UnitConverterLinear(coefficient: 0.55555555555556, constant: 255.37222222222427)
```

```
NSUnitConverter *kelvinToFahrenheit = [[NSUnitConverterLinear alloc] initWithCoefficient:0.55555555555556 constant:255.37222222222427];
```

Units that perform conversion using only a scale factor have a coefficient equal to the scale factor and a constant equal to `0`. For example, consider the kilometers unit UnitLength defines. The baseUnitValue(fromValue:) method calculates the value in meters using the formula `valueInMeters = 1000 * valueInKilometers + 0`. The value(fromBaseUnitValue:) calculates the value in kilometers using the formula `valueInKilometers = (valueInMeters - 0) / 1000`, where the coefficient is `1000` and the constant is `0`.

- Swift
- Objective-C

```
let kilometersToMeters = UnitConverterLinear(coefficient: 1000.0, constant: 0.0)
```

```
NSUnitConverterLinear *kilometersToMeters = [[NSUnitConverterLinear alloc] initWithCoefficient:1000.0 constant:0.0];
```

## Topics

### Accessing Linear Parameters

var coefficient: Double

The coefficient to use in the linear unit conversion calculation.

var constant: Double

The constant to use in the linear unit conversion calculation.

### Creating Unit Converters

convenience init(coefficient: Double)

Initializes the unit converter with the coefficient you specify.

init(coefficient: Double, constant: Double)

Creates a unit converter with the coefficient and constant you specify.

## Relationships

### Inherits From

- UnitConverter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Conversion

class UnitConverter

An abstract class that provides a description of how to convert a unit to and from the base unit of its dimension.

