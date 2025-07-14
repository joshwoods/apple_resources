

- Foundation
-  UnitPower 

Class

# UnitPower

A unit of measure for power.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitPower
```

## Overview

You typically use instances of UnitPower to represent specific quantities of power using the NSMeasurement class.

### Power

Power is the amount of energy used over time. The SI unit for power is the watt (W), which is derived as one joule per second (1W = 1J / 1s).

The UnitPower class defines its baseUnit() as watts, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Terawatts | terawatts | TW | `1e12` |
| Gigawatts | gigawatts | GW | `1e9` |
| Megawatts | megawatts | MW | `1000000.0` |
| Kilowatts | kilowatts | kW | `1000.0` |
| Watts | watts | W | `1` |
| Milliwatts | milliwatts | mW | `0.001` |
| Microwatts | microwatts | µW | `0.000001` |
| Nanowatts | nanowatts | nW | `1e-9` |
| Picowatts | picowatts | pW | `1e-12` |
| Femtowatts | femtowatts | fW | `1e-15` |
| Horsepower | horsepower | hp | `745.7` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var terawatts: UnitPower

The terawatts unit of power.

class var gigawatts: UnitPower

The gigawatts unit of power.

class var megawatts: UnitPower

The megawatts unit of power.

class var kilowatts: UnitPower

The kilowatts unit of power.

class var watts: UnitPower

The watts unit of power.

class var milliwatts: UnitPower

The milliwatts unit of power.

class var microwatts: UnitPower

The microwatts unit of power.

class var nanowatts: UnitPower

The nanowatts unit of power.

class var picowatts: UnitPower

The picowatts unit of power.

class var femtowatts: UnitPower

The femtowatts unit of power.

class var horsepower: UnitPower

The horsepower unit of power.

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

class UnitTemperature

A unit of measure for temperature.

class UnitIlluminance

A unit of measure for illuminance.

