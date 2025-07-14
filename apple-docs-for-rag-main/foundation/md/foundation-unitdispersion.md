

- Foundation
-  UnitDispersion 

Class

# UnitDispersion

A unit of measure for specific quantities of dispersion.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitDispersion
```

## Overview

You typically use instances of UnitDispersion to represent specific quantities of dispersion using the NSMeasurement class.

### Dispersion

Dispersion describes the amount of a constituent divided by the amount of all other constituents in a mixture. Dispersion is a dimensionless quantity that is commonly expressed in “parts-per” notation, such as “parts per million” (ppm), to describe small relative quantities.

The UnitDispersion class defines its baseUnit() as partsPerMillion.

| Name | Method | Abbreviation |
|----|----|----|
| Parts Per Million | partsPerMillion | ppm |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var partsPerMillion: UnitDispersion

The parts per million unit.

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

class UnitConcentrationMass

A unit of measure for concentration of mass.

