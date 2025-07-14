

- Foundation
-  UnitArea 

Class

# UnitArea

A unit of measure for area.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitArea
```

## Overview

You typically use instances of UnitArea to represent specific quantities of area using the NSMeasurement class.

### Area

Area is a quantity of extent in two dimensions. Area can be expressed by SI derived units in terms of square meters (m2). Area is also commonly measured in square feet (ft2) and acres (ac).

The UnitArea class defines its baseUnit() as squareMeters, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Square Megameters | squareMegameters | Mm² | `1e12` |
| Square Kilometers | squareKilometers | km² | `1000000.0` |
| Square Meters | squareMeters | m² | `1.0` |
| Square Centimeter | squareCentimeters | cm² | `0.0001` |
| Square Millimeters | squareMillimeters | mm² | `0.000001` |
| Square Micrometers | squareMicrometers | µm² | `1e-12` |
| Square Nanometers | squareNanometers | nm² | `1e-18` |
| Square Inches | squareInches | in² | `0.00064516` |
| Square Feet | squareFeet | ft² | `0.092903` |
| Square Yards | squareYards | yd² | `0.836127` |
| Square Miles | squareMiles | mi² | `2.59e+6` |
| Acres | acres | ac | `4046.86` |
| Ares | ares | a | `100` |
| Hectares | hectares | ha | `10000` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var squareMegameters: UnitArea

The square megameters unit of area.

class var squareKilometers: UnitArea

The square kilometers unit of area.

class var squareMeters: UnitArea

The square meters unit of area.

class var squareCentimeters: UnitArea

The square centimeters unit of area.

class var squareMillimeters: UnitArea

The square millimeters unit of area.

class var squareMicrometers: UnitArea

The square micrometers unit of area.

class var squareNanometers: UnitArea

The square nanometers unit of area.

class var squareInches: UnitArea

The square inches unit of area.

class var squareFeet: UnitArea

The square feet unit of area.

class var squareYards: UnitArea

The square yards unit of area.

class var squareMiles: UnitArea

The square miles unit of area.

class var acres: UnitArea

The acres unit of area.

class var ares: UnitArea

The ares unit of area.

class var hectares: UnitArea

The hectares unit of area.

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

### Physical Dimension

class UnitLength

A unit of measure for length.

class UnitVolume

A unit of measure for volume.

class UnitAngle

A unit of measure for planar angle and rotation.

