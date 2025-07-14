

- Foundation
-  UnitElectricCharge 

Class

# UnitElectricCharge

A unit of measure for electric charge.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitElectricCharge
```

## Overview

You typically use instances of UnitElectricCharge to represent specific quantities of electric charge using the NSMeasurement class.

### Electric Charge

Electric charge is a fundamental physical property of matter that causes it to experience a force within an electromagnetic field. The SI unit for electric charge is the coulomb (C), which is defined as the amount of charge carried by a current of one ampere in one second (1C = 1A · 1s). Charge is also commonly expressed in terms of ampere hours (Ah).

The UnitElectricCharge class defines its baseUnit() as coulombs, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Coulombs | coulombs | C | `1.0` |
| Megaampere Hours | megaampereHours | MAh | `3.6e9` |
| Kiloampere Hours | kiloampereHours | kAh | `3600000.0` |
| Ampere Hours | ampereHours | Ah | `3600.0` |
| Milliampere Hours | milliampereHours | mAh | `3.6` |
| Microampere Hours | microampereHours | µAh | `0.0036` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var coulombs: UnitElectricCharge

The coulombs unit of electric charge.

class var megaampereHours: UnitElectricCharge

The megaampere hours unit of electric charge.

class var kiloampereHours: UnitElectricCharge

The kiloampere hours unit of electric charge.

class var ampereHours: UnitElectricCharge

The ampere hours unit of electric charge.

class var milliampereHours: UnitElectricCharge

The milliampere hours unit of electric charge.

class var microampereHours: UnitElectricCharge

The microampere hours unit of electric charge.

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

class UnitElectricCurrent

A unit of measure for electric current.

class UnitElectricPotentialDifference

A unit of measure for electric potential difference.

class UnitElectricResistance

A unit of measure for electric resistance.

