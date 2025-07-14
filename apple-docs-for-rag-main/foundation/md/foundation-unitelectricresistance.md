

- Foundation
-  UnitElectricResistance 

Class

# UnitElectricResistance

A unit of measure for electric resistance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitElectricResistance
```

## Overview

You typically use instances of UnitElectricResistance to represent specific quantities of electric resistance using the NSMeasurement class.

### Electric Resistance

Electric resistance is the difficulty of passing an electric current through a conductor. The SI unit for electric resistance is the ohm (Ω), which is derived as the electric resistance that produces one ampere of current between two points in conductor with one volt of electric potential difference (1Ω = 1V/1A).

The UnitElectricResistance class defines its baseUnit() as ohms, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Megaohms | megaohms | MΩ | `1000000.0` |
| Kiloohms | kiloohms | kΩ | `1000.0` |
| Ohms | ohms | Ω | `1.0` |
| Milliohms | milliohms | mΩ | `0.001` |
| Microohms | microohms | µΩ | `0.000001` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var megaohms: UnitElectricResistance

The megaohms unit of electric resistance.

class var kiloohms: UnitElectricResistance

The kiloohms unit of electric resistance.

class var ohms: UnitElectricResistance

The ohms unit of electric resistance.

class var milliohms: UnitElectricResistance

The milliohms unit of electric resistance.

class var microohms: UnitElectricResistance

The microohms unit of electric resistance.

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

### Electricity

class UnitElectricCharge

A unit of measure for electric charge.

class UnitElectricCurrent

A unit of measure for electric current.

class UnitElectricPotentialDifference

A unit of measure for electric potential difference.

