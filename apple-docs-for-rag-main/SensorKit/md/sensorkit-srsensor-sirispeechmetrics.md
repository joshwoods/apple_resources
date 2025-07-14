

- SensorKit
- SRSensor
-  siriSpeechMetrics 

Type Property

# siriSpeechMetrics

A sensor that provides data describing a user’s speech to Siri.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let siriSpeechMetrics: SRSensor
```

## Discussion

The sample type for this sensor is SRSpeechMetrics.

The metrics provide details about the user’s voice, such as tenor, pitch, cadence, and speech timing, which includes words per minute and the average duration between words.

This sensor doesn’t provide raw audio data. For user privacy, SensorKit removes any transcript strings from the result.

You need to provide a reason to analyze speech by adding the SRSensorUsageSpeechMetrics dictionary to the NSSensorKitUsageDetail key in the information property list.

## See Also

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

