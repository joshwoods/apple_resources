

- Foundation
-  UnitPressure 

Class

# UnitPressure

A unit of measure for pressure.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitPressure
```

## Overview

You typically use instances of UnitPressure to represent specific quantities of pressure using the NSMeasurement class.

### Pressure

Pressure is the normal force over a surface. The SI unit for pressure is the pascal (Pa), which is derived as one newton of force over one square meter (`1 Pa = 1 N / 1 m`2).

The UnitPressure class defines its baseUnit() as newtonsPerMetersSquared and provides the following units, which UnitConverterLinear converters initialize with the given coefficients:

| Name | Method | Symbol | Definition |
|----|----|----|----|
| Newtons Per Meter Squared (Equivalent to Pascals) | newtonsPerMetersSquared | N/m² | `1.0` |
| Gigapascals | gigapascals | GPa | `1e9` |
| Megapascals | megapascals | MPa | `1000000.0` |
| Kilopascals | kilopascals | kPa | `1000.0` |
| Hectopascals | hectopascals | hPa | `100.0` |
| Inches of Mercury | inchesOfMercury | inHg | `3386.39` |
| Bars | bars | bar | `100000` |
| Millibars | millibars | mbar | `100` |
| Millimeters of Mercury | millimetersOfMercury | mmHg | `133.322` |
| Pounds Per Square Inch | poundsForcePerSquareInch | psi | `6894.76` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var gigapascals: UnitPressure

The gigapascals unit of pressure.

class var megapascals: UnitPressure

The megapascals unit of pressure.

class var kilopascals: UnitPressure

The kilopascals unit of pressure.

class var hectopascals: UnitPressure

The hectopascals unit of pressure.

class var inchesOfMercury: UnitPressure

The inches of mercury unit of pressure.

class var bars: UnitPressure

The bars unit of pressure.

class var millibars: UnitPressure

The millibars unit of pressure.

class var millimetersOfMercury: UnitPressure

The millimeters of mercury unit of pressure.

class var newtonsPerMetersSquared: UnitPressure

The newtons per square meter unit of pressure.

class var poundsForcePerSquareInch: UnitPressure

The pounds per square inch unit of pressure.

### Initializers

convenience init(forLocale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitPressure>)

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

### Mass, Weight, and Force

class UnitMass

A unit of measure for mass.

