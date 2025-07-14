

- HealthKit
- HKCategoryTypeIdentifier
-  environmentalAudioExposureEvent 

Type Property

# environmentalAudioExposureEvent

A category sample type that records exposure to potentially damaging sounds from the environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
static let environmentalAudioExposureEvent: HKCategoryTypeIdentifier
```

## Discussion

Apple Watch saves a environmentalAudioExposureEvent sample when it generates a *noise notification*, sent when the average sound level reaches or exceeds a specified threshold for three minutes. Apple Watch doesn’t record or save any sounds. Users can enable or disable these notifications, or set the threshold from Settings \> Noise.

Environmental audio exposure event samples are read-only. You can request permission to read the samples using this identifier, but you can’t request authorization to share them. This means you can’t save new environmental audio exposure events to the HealthKit store. To add test data in iOS Simulator, open the Health app and select Browse \> Hearing \> Noise Notifications \> Add Data.

Samples of this type use values from the HKCategoryValueEnvironmentalAudioExposureEvent enumeration.

## See Also

### Hearing

static let environmentalAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure to sounds in the environment.

static let headphoneAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure from headphones.

static let headphoneAudioExposureEvent: HKCategoryTypeIdentifier

A category sample type that records exposure to potentially damaging sounds from headphones.

static let audioExposureEvent: HKCategoryTypeIdentifier

A category sample type for audio exposure events.

Deprecated

