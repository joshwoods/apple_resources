

- HealthKit
- HKAudiogramSample
-  init(sensitivityPoints:start:end:metadata:) 

Initializer

# init(sensitivityPoints:start:end:metadata:)

Creates a new audiogram sample.

iOS 13.0–18.1DeprecatediPadOS 13.0–18.1DeprecatedMac Catalyst 13.1–18.1DeprecatedmacOS 13.0+visionOS 1.0–2.1DeprecatedwatchOS 6.0–11.1Deprecated

``` source
convenience init(
    sensitivityPoints: [HKAudiogramSensitivityPoint],
    start startDate: Date,
    end endDate: Date,
    metadata: [String : Any]?
)
```

## Parameters 

`sensitivityPoints`  

An array of sensitivity points.

`startDate`  

The start date for the sample. This date must be equal to or earlier than the end date; otherwise, this method throws an exception (invalidArgumentException).

`endDate`  

The end date for the sample. This date must be equal to or later than the start date; otherwise, this method throws an exception (invalidArgumentException).

`metadata`  

The metadata dictionary contains extra information describing this sample. The dictionary’s keys are strings. The values may be strings, numbers, or dates. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own, custom keys as needed to extend the HealthKit quantity sample’s capabilities.

