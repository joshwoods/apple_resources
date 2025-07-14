

- Foundation
-  UnitSpeed 

Class

# UnitSpeed

A unit of measure for speed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitSpeed
```

## Overview

You typically use instances of UnitSpeed to represent specific quantities of speed using the NSMeasurement class.

### Speed

Speed is the magnitude of velocity, or the rate of change of position. Speed can be expressed by SI derived units in terms of meters per second (m/s), and is also commonly expressed in terms of kilometers per hour (km/h) and miles per hour (mph).

The UnitSpeed class defines its baseUnit() as metersPerSecond, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Meters Per Second | metersPerSecond | m/s | `1.0` |
| Kilometers Per Hour | kilometersPerHour | km/h | `0.277778` |
| Miles Per Hour | milesPerHour | mph | `0.44704` |
| Knots | knots | kn | `0.514444` |

The base unit is metersPerSecond and is accessed via baseUnit() on the Dimension protocol.

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var metersPerSecond: UnitSpeed

The meter per second unit of speed.

class var kilometersPerHour: UnitSpeed

The kilometers per hour unit of speed.

class var milesPerHour: UnitSpeed

The miles per hour unit of speed.

class var knots: UnitSpeed

The knots unit of speed.

### Initializers

convenience init(forLocale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitSpeed>)

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

class UnitFrequency

A unit of measure for frequency.

