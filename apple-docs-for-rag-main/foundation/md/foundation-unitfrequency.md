

- Foundation
-  UnitFrequency 

Class

# UnitFrequency

A unit of measure for frequency.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitFrequency
```

## Overview

You typically use instances of UnitFrequency to represent specific quantities of frequency using the NSMeasurement class.

### Frequency

Frequency is a quantity of occurrences for a repeating event over time. The SI unit for frequency is the hertz (Hz), which is a derived as one occurrence per second (`1 Hz = 1 / 1s`).

The UnitFrequency class defines its baseUnit() as hertz, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Terahertz | terahertz | THz | `1e12` |
| Gigahertz | gigahertz | GHz | `1e9` |
| Megahertz | megahertz | MHz | `1000000.0` |
| Kilohertz | kilohertz | kHz | `1000.0` |
| Hertz | hertz | Hz | `1` |
| Millihertz | millihertz | mHz | `0.001` |
| Microhertz | microhertz | µHz | `0.000001` |
| Nanohertz | nanohertz | nHz | `1e-9` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var terahertz: UnitFrequency

The terahertz unit of frequency.

class var gigahertz: UnitFrequency

The gigahertz unit of frequency.

class var megahertz: UnitFrequency

The megahertz unit of frequency.

class var kilohertz: UnitFrequency

The kilohertz unit of frequency.

class var hertz: UnitFrequency

The hertz unit of frequency.

class var millihertz: UnitFrequency

The millihertz unit of frequency.

class var microhertz: UnitFrequency

The microhertz unit of frequency.

class var nanohertz: UnitFrequency

The nanohertz unit of frequency.

class var framesPerSecond: UnitFrequency

The frames per second unit of frequency.

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

### Time and Motion

class UnitAcceleration

A unit of measure for acceleration.

class UnitDuration

A unit of measure for a duration of time.

class UnitSpeed

A unit of measure for speed.

