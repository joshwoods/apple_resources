

- HealthKit
- HKAudiogramSensitivityPoint
-  init(frequency:leftEarSensitivity:rightEarSensitivity:) Deprecated

Initializer

# init(frequency:leftEarSensitivity:rightEarSensitivity:)

Creates a new sensitivity point.

iOS 13.0–18.1DeprecatediPadOS 13.0–18.1DeprecatedMac Catalyst 13.1–18.1DeprecatedmacOS 13.0+visionOS 1.0–2.1DeprecatedwatchOS 6.0–11.1Deprecated

``` source
convenience init(
    frequency: HKQuantity,
    leftEarSensitivity: HKQuantity?,
    rightEarSensitivity: HKQuantity?
) throws
```

Deprecated

Use +\[HKAudiogramSensitivityPoint sensitivityPointWithFrequency:tests:error:\]

## Parameters 

`frequency`  

The frequency tested. This object uses hertz() units.

`leftEarSensitivity`  

The sensitivity of the left ear, measured in attenuated dB from a baseline of 0 db. This object uses decibelHearingLevel() units.

`rightEarSensitivity`  

The sensitivity of the right ear, measured in attenuated dB from a baseline of 0 db. This object uses decibelHearingLevel() units.

