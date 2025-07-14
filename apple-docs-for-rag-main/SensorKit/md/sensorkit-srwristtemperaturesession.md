

- SensorKit
-  SRWristTemperatureSession 

Class

# SRWristTemperatureSession

An object that represents wrist temperatures that a device records during a period of time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
class SRWristTemperatureSession
```

## Overview

Use the startDate and duration properties to get the range of time of the measurements. Use the temperatures property to get the sequence of measurements.

## Topics

### Getting session information

var startDate: Date

The time that the device records the wrist temperature.

var duration: TimeInterval

The number of seconds that the device records the temperature.

var version: String

The version of the algorithm that analyzes the temperature.

### Getting recorded temperatures

var temperatures: some Sequence&lt;SRWristTemperature>

The wrist temperatures and their accuracies.

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

class SRWristTemperature

The temperature of the user’s wrist while the user sleeps.

