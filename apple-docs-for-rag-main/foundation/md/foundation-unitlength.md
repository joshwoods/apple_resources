

- Foundation
-  UnitLength 

Class

# UnitLength

A unit of measure for length.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitLength
```

## Overview

You typically use instances of UnitLength to represent specific quantities of length using the NSMeasurement class.

### Length

Length is the dimensional extent of matter. The SI unit for length is the meter (m), which is defined in terms of the distance traveled by light in a vacuum.

The UnitLength class defines its baseUnit() as meters, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Megameters | megameters | Mm | `1000000.0` |
| Kilometers | kilometers | kM | `1000.0` |
| Hectometers | hectometers | hm | `100.0` |
| Decameters | decameters | dam | `10.0` |
| Meters | meters | m | `1.0` |
| Decimeters | decimeters | dm | `0.1` |
| Centimeters | centimeters | cm | `0.01` |
| Millimeters | millimeters | mm | `0.001` |
| Micrometers | micrometers | µm | `0.000001` |
| Nanometers | nanometers | nm | `1e-9` |
| Picometers | picometers | pm | `1e-12` |
| Inches | inches | in | `0.0254` |
| Feet | feet | ft | `0.3048` |
| Yards | yards | yd | `0.9144` |
| Miles | miles | mi | `1609.34` |
| Scandinavian Miles | scandinavianMiles | smi | `10000` |
| Light Years | lightyears | ly | `9.461e+15` |
| Nautical Miles | nauticalMiles | NM | `1852` |
| Fathoms | fathoms | ftm | `1.8288` |
| Furlongs | furlongs | fur | `201.168` |
| Astronomical Units | astronomicalUnits | ua | `1.496e+11` |
| Parsecs | parsecs | pc | `3.086e+16` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var megameters: UnitLength

The megameters unit of length.

class var kilometers: UnitLength

The kilometers unit of length.

class var hectometers: UnitLength

The hectometers unit of length.

class var decameters: UnitLength

The decameters unit of length.

class var meters: UnitLength

The meters unit of length.

class var decimeters: UnitLength

The decimeters unit of length.

class var centimeters: UnitLength

The centimeters unit of length.

class var millimeters: UnitLength

The millimeters unit of length.

class var micrometers: UnitLength

The micrometers unit of length.

class var nanometers: UnitLength

The nanometers unit of length.

class var picometers: UnitLength

The picometers unit of length.

class var inches: UnitLength

The inches unit of length.

class var feet: UnitLength

The feet unit of length.

class var yards: UnitLength

The yards unit of length.

class var miles: UnitLength

The miles unit of length.

class var scandinavianMiles: UnitLength

The Scandinavian miles unit of length.

class var lightyears: UnitLength

The light years unit of length.

class var nauticalMiles: UnitLength

The nautical miles unit of length.

class var fathoms: UnitLength

The fathoms unit of length.

class var furlongs: UnitLength

The furlongs unit of length.

class var astronomicalUnits: UnitLength

The astronomical units unit of length.

class var parsecs: UnitLength

The parsecs unit of length.

### Initializers

convenience init(forLocale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitLength>)

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

class UnitVolume

A unit of measure for volume.

class UnitAngle

A unit of measure for planar angle and rotation.

