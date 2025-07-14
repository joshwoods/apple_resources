

- Foundation
-  UnitIlluminance 

Class

# UnitIlluminance

A unit of measure for illuminance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitIlluminance
```

## Overview

You typically use instances of UnitIlluminance to represent specific quantities of illuminance using the NSMeasurement class.

### Illuminance

Illuminance is the luminous flux incident on a surface. The SI unit for illuminance is the lux (lx), which is derived as one lumen per square meter (1lm / 1m2).

The UnitIlluminance class defines its baseUnit() as lux.

| Name | Method | Symbol |
|----|----|----|
| Lux | lux | lx |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accesing Predefined Units

class var lux: UnitIlluminance

The lux unit of illuminance.

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

### Energy, Heat, and Light

class UnitEnergy

A unit of measure for energy.

class UnitPower

A unit of measure for power.

class UnitTemperature

A unit of measure for temperature.

