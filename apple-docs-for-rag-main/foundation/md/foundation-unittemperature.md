

- Foundation
-  UnitTemperature 

Class

# UnitTemperature

A unit of measure for temperature.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitTemperature
```

## Overview

You typically use instances of UnitTemperature to represent specific quantities of temperature using the NSMeasurement class.

### Temperature

Temperature is a comparative measure of thermal energy. The SI unit for temperature is the kelvin (K), which is defined in terms of the triple point of water. Temperature is also commonly measured by degrees of various scales, including Celsius (°C) and Fahrenheit (°F).

The UnitTemperature class defines its baseUnit() to be kelvin, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients and constants:

| Name | Method | Symbol | Coefficient | Constant |
|----|----|----|----|----|
| Kelvin | kelvin | K | `1` | `0` |
| Degree Celsius | celsius | °C | `1.0` | `273.15` |
| Degree Fahrenheit | fahrenheit | °F | `0.55555555555556` | `255.37222222222427` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var kelvin: UnitTemperature

The kelvin unit of temperature.

class var celsius: UnitTemperature

The degree Celsius unit of temperature.

class var fahrenheit: UnitTemperature

The degree Fahrenheit unit of temperature.

### Initializers

convenience init(forLocale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitTemperature>)

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

class UnitIlluminance

A unit of measure for illuminance.

