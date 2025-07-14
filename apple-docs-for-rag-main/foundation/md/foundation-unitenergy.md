

- Foundation
-  UnitEnergy 

Class

# UnitEnergy

A unit of measure for energy.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitEnergy
```

## Overview

You typically use instances of UnitEnergy to represent specific quantities of energy using the NSMeasurement class.

### Energy

Energy is a fundamental property of matter than can be transferred and converted into different forms, such as kinetic, electric, and thermal. The SI unit for energy is the joule (J), which is derived as the work of one meter of displacement in the direction of a force of one newton (1J = 1N ∙ 1m). It can also be derived as the work required to displace an electric charge of one coulomb through an electrical potential difference of one volt (1J = 1C ∙ 1V), or the work required to produce one watt of power for one second (1J = 1W ∙ 1s). Energy is also commonly expressed in terms of the calorie (cal), or the energy needed to raise the temperature of one gram of water by one degree Celsius at a pressure of one atmosphere (1cal ≡ 4.184J).

The UnitEnergy class defines its baseUnit() as joules, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Kilojoules | kilojoules | kJ | `1000.0` |
| Joules | joules | J | `1.0` |
| Kilocalories | kilocalories | kCal | `4184.0` |
| Calories | calories | cal | `4.184` |
| Kilowatt Hours | kilowattHours | kWh | `3600000.0` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var kilojoules: UnitEnergy

The kilojoules unit of energy.

class var joules: UnitEnergy

The joules unit of energy.

class var kilocalories: UnitEnergy

The kilocalories unit of energy.

class var calories: UnitEnergy

The calories unit of energy.

class var kilowattHours: UnitEnergy

The kilowatt hours unit of energy.

### Initializers

convenience init(forLocale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitEnergy>)

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

class UnitPower

A unit of measure for power.

class UnitTemperature

A unit of measure for temperature.

class UnitIlluminance

A unit of measure for illuminance.

