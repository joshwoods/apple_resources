

- SensorKit
-  SRPhotoplethysmogramAccelerometerSample 

Class

# SRPhotoplethysmogramAccelerometerSample

A data sample from the photoplethysmogram (PPG) accelerometer.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
class SRPhotoplethysmogramAccelerometerSample
```

## Topics

### Accessing accelerometer data

var nanosecondsSinceStart: Int64

The time in nanoseconds since the start of the accelerometer data recording.

var samplingFrequency: Measurement&lt;UnitFrequency>

The frequency of the accelerometer data recording in hertz.

var x: Measurement&lt;UnitAcceleration>

The x-axis acceleration in G’s (gravitational force).

var y: Measurement&lt;UnitAcceleration>

The y-axis acceleration in G’s (gravitational force).

var z: Measurement&lt;UnitAcceleration>

The z-axis acceleration in G’s (gravitational force).

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

var temperature: Measurement&lt;UnitTemperature>?

The samples recorded by the photoplethysmogram (PPG) thermometer.

