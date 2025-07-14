

- SensorKit
- SRFetchResult
-  sample 

Instance Property

# sample

A recording that the sensor reader fetches.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
@NSCopying
var sample: SampleType { get }
```

## Discussion

The framework expects the app to know the result type based on the reader’s sensor.

### Sample types

This property’s type is a superclass from which the framework derives discrete sample types. Depending on the sensor associated with your app’s sensor reader, type cast the fetch result’s sample to the sensor’s associated sample type. The following list provides the sample type per sensor:

accelerometer  
\[CMRecordedAccelerometerData\]

ambientLightSensor  
SRAmbientLightSample

ambientPressure  
`[`CMRecordedPressureData`]`

deviceUsageReport  
SRDeviceUsageReport

faceMetrics  
SRFaceMetrics

heartRate  
CMHighFrequencyHeartRateData

keyboardMetrics  
SRKeyboardMetrics

mediaEvents  
SRMediaEvent

messagesUsageReport  
SRMessagesUsageReport

odometer  
CMOdometerData

onWristState  
SRWristDetection

pedometerData  
CMPedometerData

phoneUsageReport  
SRPhoneUsageReport

rotationRate  
\[CMRecordedRotationRateData\]

siriSpeechMetrics  
SRSpeechMetrics

telephonySpeechMetrics  
SRSpeechMetrics

visits  
SRVisit

wristTemperature  
SRWristTemperature

## See Also

### Sampling Data

var timestamp: SRAbsoluteTime

The time when the framework records the sample.

