

- HealthKit
- HKQuantityTypeIdentifier
-  environmentalAudioExposure 

Type Property

# environmentalAudioExposure

A quantity sample type that measures audio exposure to sounds in the environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let environmentalAudioExposure: HKQuantityTypeIdentifier
```

## Discussion

These samples use sound pressure units (described in HKUnit). You create these units using the decibelAWeightedSoundPressureLevel() method. They measure discrete values of the equivalent continuous sound pressure level, described in HKQuantityAggregationStyle.discreteEquivalentContinuousLevel.

## See Also

### Hearing

static let headphoneAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure from headphones.

static let environmentalAudioExposureEvent: HKCategoryTypeIdentifier

A category sample type that records exposure to potentially damaging sounds from the environment.

static let headphoneAudioExposureEvent: HKCategoryTypeIdentifier

A category sample type that records exposure to potentially damaging sounds from headphones.

static let audioExposureEvent: HKCategoryTypeIdentifier

A category sample type for audio exposure events.

Deprecated

