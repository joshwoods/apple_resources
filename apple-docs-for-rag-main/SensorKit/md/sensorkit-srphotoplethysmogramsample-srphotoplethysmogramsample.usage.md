

- SensorKit
- SRPhotoplethysmogramSample
-  SRPhotoplethysmogramSample.Usage 

Structure

# SRPhotoplethysmogramSample.Usage

The possible ways that a person or the system may take a photoplethysmogram (PPG) reading.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
struct Usage
```

## Topics

### Getting the reading method

static let foregroundHeartRate: SRPhotoplethysmogramSample.Usage

A heart rate reading that a person takes while using an app.

static let deepBreathing: SRPhotoplethysmogramSample.Usage

A deep breathing sensor reading that a person takes while using an app.

static let foregroundBloodOxygen: SRPhotoplethysmogramSample.Usage

A blood oxygen reading that a person takes while using an app.

static let backgroundSystem: SRPhotoplethysmogramSample.Usage

A reading taken by the system in the background.

### Initializing usage

init(rawValue: String)

Initializes a PPG usage structure.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing PPG data

var startDate: Date

The start date of the photoplethysmogram (PPG) sensor data recording.

var nanosecondsSinceStart: Int64

The time in nanoseconds since the start of the data recording.

var usage: [SRPhotoplethysmogramSample.Usage]

The method that the person or system uses to take the reading.

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

