

- Foundation
-  UnitMass 

Class

# UnitMass

A unit of measure for mass.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitMass
```

## Overview

You typically use instances of UnitMass to represent specific quantities of mass using the NSMeasurement class.

### Mass

Mass is a fundamental property of matter that causes it to resist a force accelerating it. The SI unit for mass is the kilogram (kg), which defined in terms of the mass of the international prototype kilogram.

The UnitMass class defines its baseUnit() as kilograms, and provides the following units, which UnitConverterLinear converters initialize with the given coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Kilograms | kilograms | kg | `1.0` |
| Grams | grams | g | `0.001` |
| Decigrams | decigrams | dg | `0.0001` |
| Centigrams | centigrams | cg | `0.00001` |
| Milligrams | milligrams | mg | `0.000001` |
| Micrograms | micrograms | µg | `1e-9` |
| Nanograms | nanograms | ng | `1e-12` |
| Picograms | picograms | pg | `1e-15` |
| Ounces | ounces | oz | `0.0283495` |
| Pounds | pounds | lb | `0.453592` |
| Stones | stones | st | `0.157473` |
| Metric Tons | metricTons | t | `1000` |
| Short Tons | shortTons | ton | `907.185` |
| Carats | carats | ct | `0.0002` |
| Ounces Troy | ouncesTroy | oz t | `0.03110348` |
| Slugs | slugs | slug | `14.5939` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var kilograms: UnitMass

The kilograms unit of mass.

class var grams: UnitMass

The grams unit of mass.

class var decigrams: UnitMass

The decigrams unit of mass.

class var centigrams: UnitMass

The centigrams unit of mass.

class var milligrams: UnitMass

The milligrams unit of mass.

class var micrograms: UnitMass

The micrograms unit of mass.

class var nanograms: UnitMass

The nanograms unit of mass.

class var picograms: UnitMass

The picograms unit of mass.

class var ounces: UnitMass

The ounces unit of mass.

pounds

Returns the pounds unit of mass.

class var pounds: UnitMass

The pounds unit of mass.

class var stones: UnitMass

The stone unit of mass.

class var metricTons: UnitMass

The metric tons unit of mass.

class var shortTons: UnitMass

The short tons unit of mass.

class var carats: UnitMass

The carats unit of mass.

class var ouncesTroy: UnitMass

The ounces troy unit of mass.

class var slugs: UnitMass

The slugs unit of mass.

### Initializers

convenience init(forLocale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitMass>)

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

class UnitPressure

A unit of measure for pressure.

