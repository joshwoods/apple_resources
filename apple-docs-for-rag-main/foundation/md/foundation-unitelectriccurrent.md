

- Foundation
-  UnitElectricCurrent 

Class

# UnitElectricCurrent

A unit of measure for electric current.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitElectricCurrent
```

## Overview

You typically use instances of UnitElectricCurrent to represent specific quantities of electric current using the NSMeasurement class.

### Electric Current

Electric current is the flow of electric charge. The SI unit for electric current is the ampere (A), which is defined in terms the production of electromagnetic force between two parallel linear conductors. It can also be expressed as the flow of one coulomb per second (1A = 1C / s).

The UnitElectricCurrent class defines its baseUnit() as amperes, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Megaamperes | megaamperes | MA | `1000000.0` |
| Kiloamperes | kiloamperes | kA | `1000.0` |
| Amperes | amperes | A | `1.0` |
| Milliamperes | milliamperes | mA | `0.001` |
| Microamperes | microamperes | µA | `0.000001` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var megaamperes: UnitElectricCurrent

The megaamperes unit of electric current.

class var kiloamperes: UnitElectricCurrent

The kiloamperes unit of electric current.

class var amperes: UnitElectricCurrent

The amperes unit of electric current.

class var milliamperes: UnitElectricCurrent

The milliamperes unit of electric current.

class var microamperes: UnitElectricCurrent

The microamperes unit of electric current.

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

class UnitElectricPotentialDifference

A unit of measure for electric potential difference.

class UnitElectricResistance

A unit of measure for electric resistance.

