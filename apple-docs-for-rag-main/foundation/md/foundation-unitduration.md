

- Foundation
-  UnitDuration 

Class

# UnitDuration

A unit of measure for a duration of time.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitDuration
```

## Overview

You typically use instances of UnitDuration to represent specific quantities of planar angle using the NSMeasurement class.

### Duration

Duration is a quantity of time. The SI unit for time is the second (sec), which is defined in terms of the radioactivity of a cesium-133 atom. Duration is also commonly expressed in terms of minutes (min) and hours (hr).

Note

Use the NSDateComponents class to represent quantities of calendrical units, such as days, weeks, months, and years.

The UnitDuration class defines its baseUnit() as seconds, and provides the following units, which UnitConverterLinear converters initialize with the given coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Seconds | seconds | sec | `1` |
| Minutes | minutes | min | `60` |
| Hours | hours | hr | `3600` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var hours: UnitDuration

The hour unit of duration.

class var minutes: UnitDuration

The minute unit of duration.

class var seconds: UnitDuration

The second unit of duration.

class var milliseconds: UnitDuration

The millisecond unit of duration.

class var microseconds: UnitDuration

The microsecond unit of duration.

class var nanoseconds: UnitDuration

The nanosecond unit of duration.

class var picoseconds: UnitDuration

The picosecond unit of duration.

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

class UnitFrequency

A unit of measure for frequency.

class UnitSpeed

A unit of measure for speed.

