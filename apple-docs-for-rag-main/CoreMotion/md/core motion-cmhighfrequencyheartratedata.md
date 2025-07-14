

- Core Motion
-  CMHighFrequencyHeartRateData 

Class

# CMHighFrequencyHeartRateData

A class that represents heart rate data collected at 1 Hz.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+watchOS 10.0+

``` source
class CMHighFrequencyHeartRateData
```

## Overview

Use the heartRate property to get the data, and the confidence property for the accuracy.

## Topics

### Accessing heart rate data

var heartRate: Double

The heart rate value in units of beats per minute (BPM).

var confidence: CMHighFrequencyHeartRateDataConfidence

The confidence level of the heart rate value.

enum CMHighFrequencyHeartRateDataConfidence

The level of confidence in the accuracy of the heart rate data.

### Getting the sample date

var date: Date?

The time the heart rate value occurs.

## Relationships

### Inherits From

- CMLogItem

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

## See Also

### Pedometer and fitness

class CMPedometer

An object for fetching the system-generated live walking data.

class CMPedometerData

Information about the distance traveled by a user on foot.

class CMPedometerEvent

A change in the user’s pedestrian activity.

class CMStepCounter

The number of steps the user has taken with the device.

Deprecated

class CMOdometerData

A class that represents odometer data for workouts.

