

- HealthKit
- HKCategoryTypeIdentifier
-  headphoneAudioExposureEvent 

Type Property

# headphoneAudioExposureEvent

A category sample type that records exposure to potentially damaging sounds from headphones.

iOS 14.2+iPadOS 14.2+Mac Catalyst 14.2+macOS 13.0+visionOS 1.0+watchOS 7.1+

``` source
static let headphoneAudioExposureEvent: HKCategoryTypeIdentifier
```

## Discussion

iPhone and Apple Watch save a headphoneAudioExposureEvent sample when the device generates a notification about loud headphone audio. Both devices generate these notifications when the user listens to audio long enough and at a volume that could affect their hearing. In some regions, users can enable or disable loud headphone notifications from Settings \> Sounds & Haptics \> Headphone Safety.

Samples of this type use values from the HKCategoryValueHeadphoneAudioExposureEvent enumeration.

## Topics

### Metadata Keys

let HKMetadataKeyAudioExposureLevel: String

The audio level associated with an audio event.

let HKMetadataKeyAudioExposureDuration: String

The audio exposure event’s duration.

## See Also

### Hearing

static let environmentalAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure to sounds in the environment.

static let headphoneAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure from headphones.

static let environmentalAudioExposureEvent: HKCategoryTypeIdentifier

A category sample type that records exposure to potentially damaging sounds from the environment.

static let audioExposureEvent: HKCategoryTypeIdentifier

A category sample type for audio exposure events.

Deprecated

