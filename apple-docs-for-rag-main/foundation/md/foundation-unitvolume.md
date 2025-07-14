

- Foundation
-  UnitVolume 

Class

# UnitVolume

A unit of measure for volume.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitVolume
```

## Overview

You typically use instances of UnitVolume to represent specific quantities of volume using the NSMeasurement class.

### Volume

Volume is a quantity of the extend of matter in three dimensions. The SI accepted unit of volume is the liter (L), which is derived as one cubic decimeter (1 dm3). Volume is also commonly expressed in terms of cubic meters (m3), gallons (gal), and cups (cup).

The UnitVolume class defines its baseUnit() as liters, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Megaliters | megaliters | ML | `1000000.0` |
| Kiloliters | kiloliters | kL | `1000.0` |
| Liters | liters | L | `1.0` |
| Deciliters | deciliters | dL | `0.1` |
| Centiliters | centiliters | cL | `0.01` |
| Milliliters | milliliters | mL | `0.001` |
| Cubic Kilometers | cubicKilometers | km³ | `1e12` |
| Cubic Meters | cubicMeters | m³ | `1000.0` |
| Cubic Decimeters | cubicDecimeters | dm³ | `1.0` |
| Cubic Millimeters | cubicMillimeters | mm³ | `0.000001` |
| Cubic Inches | cubicInches | in³ | `0.0163871` |
| Cubic Feet | cubicFeet | ft³ | `28.3168` |
| Cubic Yards | cubicYards | yd³ | `764.555` |
| Cubic Miles | cubicMiles | mi³ | `4.168e+12` |
| Acre Foeet | acreFeet | af | `1.233e+6` |
| Bushels | bushels | bsh | `35.2391` |
| Teaspoons | teaspoons | tsp | `0.00492892` |
| Tablespoons | tablespoons | tbsp | `0.0147868` |
| Fluid Ounces | fluidOunces | fl oz | `0.0295735` |
| Cups | cups | cup | `0.24` |
| Pints | pints | pt | `0.473176` |
| Quarts | quarts | qt | `0.946353` |
| Gallons | gallons | gal | `3.78541` |
| Imperial Teaspoons | imperialTeaspoons | tsp | `0.00591939` |
| Imperial Tablespoons | imperialTablespoons | tbsp | `0.0177582` |
| Imperial Fluid Ounces | imperialFluidOunces | fl oz | `0.0284131` |
| Imperial Pints | imperialPints | pt | `0.568261` |
| Imperial Quarts | imperialQuarts | qt | `1.13652` |
| Imperial Gallons | imperialGallons | gal | `4.54609` |
| Metric Cups | metricCups | metric cup | `0.25` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var megaliters: UnitVolume

The megaliters unit of volume.

class var kiloliters: UnitVolume

The kiloliters unit of volume.

class var liters: UnitVolume

The liters unit of volume.

class var deciliters: UnitVolume

The deciliters unit of volume.

class var centiliters: UnitVolume

The centiliters unit of volume.

class var milliliters: UnitVolume

The milliliters unit of volume.

class var cubicKilometers: UnitVolume

The cubic kilometers unit of volume.

class var cubicMeters: UnitVolume

The cubic meters unit of volume.

class var cubicDecimeters: UnitVolume

The cubic decimeters unit of volume.

class var cubicCentimeters: UnitVolume

The cubic centimeters unit of volume.

class var cubicMillimeters: UnitVolume

The cubic millimeters unit of volume.

class var cubicInches: UnitVolume

The cubic inches unit of volume.

class var cubicFeet: UnitVolume

The cubic feet unit of volume.

class var cubicYards: UnitVolume

The cubic yards unit of volume.

class var cubicMiles: UnitVolume

The cubic miles unit of volume.

class var acreFeet: UnitVolume

The acre feet unit of volume.

class var bushels: UnitVolume

The bushels unit of volume.

class var teaspoons: UnitVolume

The teaspoons unit of volume.

class var tablespoons: UnitVolume

The tablespoons unit of volume.

class var fluidOunces: UnitVolume

The fluid ounces unit of volume.

class var cups: UnitVolume

The cups unit of volume.

class var pints: UnitVolume

The pints unit of volume.

class var quarts: UnitVolume

The quarts unit of volume.

class var gallons: UnitVolume

The gallons unit of volume.

class var imperialTeaspoons: UnitVolume

The imperial teaspoons unit of volume.

class var imperialTablespoons: UnitVolume

The imperial tablespoons unit of volume.

class var imperialFluidOunces: UnitVolume

The imperial fluid ounces unit of volume.

class var imperialPints: UnitVolume

The imperial pints unit of volume.

class var imperialQuarts: UnitVolume

The imperial quarts unit of volume.

class var imperialGallons: UnitVolume

The imperial gallons unit of volume.

class var metricCups: UnitVolume

The metric cups unit of volume.

### Initializers

convenience init(forLocale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitVolume>)

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

class UnitArea

A unit of measure for area.

class UnitLength

A unit of measure for length.

class UnitAngle

A unit of measure for planar angle and rotation.

