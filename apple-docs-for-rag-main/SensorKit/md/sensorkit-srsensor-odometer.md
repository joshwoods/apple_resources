

- SensorKit
- SRSensor
-  odometer 

Type Property

# odometer

A sensor that provides information about speed and slope.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
static let odometer: SRSensor
```

## Discussion

The sample type for this sensor is CMOdometerData.

You need to provide a reason to record the user’s odometer by adding the SRSensorUsageOdometer dictionary to the NSSensorKitUsageDetail key in the information property list.

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

