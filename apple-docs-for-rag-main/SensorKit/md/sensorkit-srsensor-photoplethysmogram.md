

- SensorKit
- SRSensor
-  photoplethysmogram 

Type Property

# photoplethysmogram

A sensor that streams sample PPG sensor data.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
static let photoplethysmogram: SRSensor
```

## Discussion

The sample for this sensor is an array of SRPhotoplethysmogramSample objects.

You need to provide a reason to record photoplethysmogram (PPG) data by adding the `SRSensorUsagePPG` dictionary to the NSSensorKitUsageDetail key in the information property list.

You also need the `ppg` key added to the `com.apple.developer.sensorkit.reader.allow` entitlement, as in:

```

        com.apple.developer.sensorkit.reader.allow

                ppg

```

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

static let siriSpeechMetrics: SRSensor

A sensor that provides data describing a user’s speech to Siri.

static let telephonySpeechMetrics: SRSensor

A sensor that provides data describing speech during phone calls.

static let visits: SRSensor

A sensor that provides information about frequently visited locations.

static let wristTemperature: SRSensor

A sensor that provides wrist temperature while the user sleeps.

static let electrocardiogram: SRSensor

A sensor that streams sample ECG sensor data.

