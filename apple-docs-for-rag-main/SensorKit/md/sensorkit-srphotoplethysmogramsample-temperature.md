

- SensorKit
- SRPhotoplethysmogramSample
-  temperature 

Instance Property

# temperature

The samples recorded by the photoplethysmogram (PPG) thermometer.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var temperature: Measurement? { get }
```

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

class SRPhotoplethysmogramAccelerometerSample

A data sample from the photoplethysmogram (PPG) accelerometer.

