

- Foundation
-  UnitAcceleration 

Class

# UnitAcceleration

A unit of measure for acceleration.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitAcceleration
```

## Overview

You typically use instances of UnitAcceleration to represent specific quantities of acceleration using the NSMeasurement class.

### Acceleration

Acceleration is the rate of change of velocity. Acceleration can be expressed by SI derived units in terms of meters per second squared (m/s2).

The UnitAcceleration class defines its baseUnit() as metersPerSecondSquared, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Meters Per Second Squared | metersPerSecondSquared | m/s² | `1.0` |
| Gravity | gravity | g | `9.81` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var metersPerSecondSquared: UnitAcceleration

Returns the meter per second squared unit of acceleration.

class var gravity: UnitAcceleration

Returns the gravity unit of acceleration.

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

class UnitDuration

A unit of measure for a duration of time.

class UnitFrequency

A unit of measure for frequency.

class UnitSpeed

A unit of measure for speed.

