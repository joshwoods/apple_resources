

- SensorKit
-  SRPhotoplethysmogramSample 

Class

# SRPhotoplethysmogramSample

The sample photoplethysmogram (PPG) sensor data.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
class SRPhotoplethysmogramSample
```

## Overview

The PPG sensor provides an array of these objects as its sample type.

Apple Watch uses LED lights, paired with light-sensitive photodiodes (PD), to track the heartbeat-induced pulsations. Different Apple Watch models can have different numbers of LEDs and PDs. For more information, see SRPhotoplethysmogramOpticalSample.

For more details, see:

- Monitor your heart rate with Apple Watch

- Using Apple Watch for Arrhythmia Detection

- How to use the Blood Oxygen app on Apple Watch

- Blood Oxygen app on Apple Watch

## Topics

### Accessing PPG data

var startDate: Date

The start date of the photoplethysmogram (PPG) sensor data recording.

var nanosecondsSinceStart: Int64

The time in nanoseconds since the start of the data recording.

var usage: [SRPhotoplethysmogramSample.Usage]

The method that the person or system uses to take the reading.

struct Usage

The possible ways that a person or the system may take a photoplethysmogram (PPG) reading.

var opticalSamples: [SRPhotoplethysmogramOpticalSample]

The samples recorded by the photoplethysmogram (PPG) optical sensor.

class SRPhotoplethysmogramOpticalSample

A data sample from the photoplethysmogram (PPG) optical sensor.

var accelerometerSamples: [SRPhotoplethysmogramAccelerometerSample]

The samples recorded by the photoplethysmogram (PPG) accelerometer.

class SRPhotoplethysmogramAccelerometerSample

A data sample from the photoplethysmogram (PPG) accelerometer.

var temperature: Measurement&lt;UnitTemperature>?

The samples recorded by the photoplethysmogram (PPG) thermometer.

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

