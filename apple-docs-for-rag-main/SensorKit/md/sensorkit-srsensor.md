

- SensorKit
-  SRSensor 

Structure

# SRSensor

The sensors an app can read.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
struct SRSensor
```

## Mentioned in 

Configuring your project for sensor reading

## Discussion

Use the properties in this structure to access the different sensors.

## Topics

### Reading device sensors

static let deviceUsageReport: SRSensor

A sensor that provides information about device usage.

static let keyboardMetrics: SRSensor

A sensor that provides information about keyboard usage.

static let onWristState: SRSensor

A sensor that describes the watch’s position on the wrist.

### Reading app activity sensors

static let messagesUsageReport: SRSensor

A sensor that provides information about use of the Messages app.

static let phoneUsageReport: SRSensor

A sensor that reports the amount of time that the user is on phone calls.

### Reading user activity sensors

static let accelerometer: SRSensor

A sensor that provides acceleration motion data.

static let faceMetrics: SRSensor

A sensor that provides data describing a user’s face.

static let heartRate: SRSensor

A sensor that provides the user’s heart rate data.

static let mediaEvents: SRSensor

A sensor that provides information about interactions with media, such as images and videos, in messaging apps.

static let odometer: SRSensor

A sensor that provides information about speed and slope.

static let pedometerData: SRSensor

A sensor that provides information about the user’s steps.

static let rotationRate: SRSensor

A sensor that provides rotation motion data.

static let siriSpeechMetrics: SRSensor

A sensor that provides data describing a user’s speech to Siri.

static let telephonySpeechMetrics: SRSensor

A sensor that provides data describing speech during phone calls.

static let visits: SRSensor

A sensor that provides information about frequently visited locations.

static let wristTemperature: SRSensor

A sensor that provides wrist temperature while the user sleeps.

static let photoplethysmogram: SRSensor

A sensor that streams sample PPG sensor data.

static let electrocardiogram: SRSensor

A sensor that streams sample ECG sensor data.

### Reading environment sensors

static let ambientLightSensor: SRSensor

A sensor that provides ambient light information.

static let ambientPressure: SRSensor

A sensor that provides pressure and temperature metrics.

### Creating a sensor

init(rawValue: String)

Creates a sensor from a raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a sensor reader

init(sensor: SRSensor)

Initializes a new sensor reader object.

var sensor: SRSensor

The particular sensor that this object reads.

