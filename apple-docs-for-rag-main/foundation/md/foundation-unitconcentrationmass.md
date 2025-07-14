

- Foundation
-  UnitConcentrationMass 

Class

# UnitConcentrationMass

A unit of measure for concentration of mass.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitConcentrationMass
```

## Overview

You typically use instances of UnitConcentrationMass to represent specific quantities of concentration using the NSMeasurement class.

### Concentration of Mass

Concentration is the abundance of a constituent within a volume. Concentration can be expressed by SI derived units in terms of kilograms per cubic meter (kg/m3).

The UnitConcentrationMass class defines its baseUnit() as gramsPerLiter, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Grams Per Liter | gramsPerLiter | g/L | `1` |
| Milligrams Per Deciliter | milligramsPerDeciliter | mg/dL | `0.01` |
| Millimoles Per Liter | millimolesPerLiter(withGramsPerMole:) | mmol/L | `18 * gramsPerMole` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var gramsPerLiter: UnitConcentrationMass

The grams per liter unit of concentration.

class var milligramsPerDeciliter: UnitConcentrationMass

The milligrams per deciliter unit of concentration.

class func millimolesPerLiter(withGramsPerMole: Double) -> UnitConcentrationMass

Returns the millimoles per liter unit with the specified number of grams per mole.

## Relationships

### Inherits From

- Dimension

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Concentration and Dispersion

class UnitDispersion

A unit of measure for specific quantities of dispersion.

