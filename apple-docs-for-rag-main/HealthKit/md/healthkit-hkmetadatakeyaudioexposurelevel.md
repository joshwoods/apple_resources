

- HealthKit
-  HKMetadataKeyAudioExposureLevel 

Global Variable

# HKMetadataKeyAudioExposureLevel

The audio level associated with an audio event.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let HKMetadataKeyAudioExposureLevel: String
```

## Discussion

Use this key on audio exposure events. It takes an HKQuantity containing the audio level measured in decibelAWeightedSoundPressureLevel() units.

