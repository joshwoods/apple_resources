

- Foundation
-  UnitFuelEfficiency 

Class

# UnitFuelEfficiency

A unit of measure for fuel efficiency.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitFuelEfficiency
```

## Overview

You typically use instances of UnitFuelEfficiency to represent specific quantities of fuel efficiency using the NSMeasurement class.

### Fuel Efficiency

Fuel efficiency corresponds to the thermal efficiency of a process that converts the chemical potential energy of a fuel into kinetic energy. Fuel efficiency can be expressed by SI derived units in terms of cubic meters per meter (m3/m), but is more commonly expressed in terms of liters per kilometer (L/km) and miles per gallon (mpg).

The UnitFuelEfficiency class defines its baseUnit() as litersPer100Kilometers, and provides the following units:

| Name | Method | Symbol |
|----|----|----|
| Liters Per 100 Kilometers | litersPer100Kilometers | L/100km |
| Miles Per Gallon | milesPerGallon | mpg |
| Miles Per Imperial Gallon | milesPerImperialGallon | mpg |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var milesPerImperialGallon: UnitFuelEfficiency

The miles per imperial gallon unit of fuel efficiency.

class var litersPer100Kilometers: UnitFuelEfficiency

The liters per 100 kilometers unit of fuel efficiency.

class var milesPerGallon: UnitFuelEfficiency

The miles per gallon unit of fuel efficiency.

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

