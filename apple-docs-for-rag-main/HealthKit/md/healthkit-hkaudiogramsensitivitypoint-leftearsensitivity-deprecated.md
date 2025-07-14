

- HealthKit
- HKAudiogramSensitivityPoint
-  leftEarSensitivity Deprecated

Instance Property

# leftEarSensitivity

The sensitivity of the left ear.

iOS 13.0–18.1DeprecatediPadOS 13.0–18.1DeprecatedMac Catalyst 13.1–18.1DeprecatedmacOS 13.0+visionOS 1.0–2.1DeprecatedwatchOS 6.0–11.1Deprecated

``` source
@NSCopying
var leftEarSensitivity: HKQuantity? { get }
```

Deprecated

Use tests object which will contain a value for left ear

## Discussion

This object uses decibelHearingLevel() units to measure sensitivity in attenuated dB from a baseline of 0 dB.

## See Also

### Accessing Data

var frequency: HKQuantity

The frequency tested in the hearing test.

var rightEarSensitivity: HKQuantity?

The sensitivity of the right ear.

Deprecated

