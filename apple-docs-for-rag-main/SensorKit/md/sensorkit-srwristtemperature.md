

- SensorKit
-  SRWristTemperature 

Class

# SRWristTemperature

The temperature of the user’s wrist while the user sleeps.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
class SRWristTemperature
```

## Overview

The wristTemperature sensor provides this class as its sample type.

## Topics

### Getting temperature information

var timestamp: Date

The date and time when the device records the temperature.

var value: Measurement&lt;UnitTemperature>

The temperature sensor value in celsius.

var errorEstimate: Measurement&lt;UnitTemperature>

An estimate of the amount of error in the temperature measurement.

### Determining the accuracy

var condition: SRWristTemperature.Condition

The condition of the measurement that impacts its accuracy.

struct Condition

The user activities with the watch that can impact the temperature measurement.

## Relationships

### Inherits From

- NSObject

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

### Recording wrist temperatures

class SRWristTemperatureSession

An object that represents wrist temperatures that a device records during a period of time.

