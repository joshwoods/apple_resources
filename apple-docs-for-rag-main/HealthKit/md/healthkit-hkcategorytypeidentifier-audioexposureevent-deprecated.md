

- HealthKit
- HKCategoryTypeIdentifier
-  audioExposureEvent Deprecated

Type Property

# audioExposureEvent

A category sample type for audio exposure events.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOSvisionOS 1.0–1.0DeprecatedwatchOS 6.0–7.0Deprecated

``` source
static let audioExposureEvent: HKCategoryTypeIdentifier
```

Deprecated

Use environmentalAudioExposureEvent instead.

## Discussion

These samples use values from HKCategoryValueAudioExposureEvent.

## Topics

### Metadata Keys

let HKMetadataKeyAudioExposureLevel: String

The audio level associated with an audio event.

## See Also

### Hearing

static let environmentalAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure to sounds in the environment.

static let headphoneAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure from headphones.

static let environmentalAudioExposureEvent: HKCategoryTypeIdentifier

A category sample type that records exposure to potentially damaging sounds from the environment.

static let headphoneAudioExposureEvent: HKCategoryTypeIdentifier

A category sample type that records exposure to potentially damaging sounds from headphones.

