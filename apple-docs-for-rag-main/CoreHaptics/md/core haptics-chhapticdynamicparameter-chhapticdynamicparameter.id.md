

- Core Haptics
- CHHapticDynamicParameter
-  CHHapticDynamicParameter.ID 

Structure

# CHHapticDynamicParameter.ID

The identifier that reveals the type of property associated with a dynamic parameter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
struct ID
```

## Topics

### Haptic Dynamic Parameter IDs

static let hapticIntensityControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the strength of a haptic pattern.

static let hapticSharpnessControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the sharpness of a haptic pattern.

static let hapticAttackTimeControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the time when a haptic pattern’s intensity begins increasing.

static let hapticDecayTimeControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the time when a haptic pattern’s intensity begins decreasing.

static let hapticReleaseTimeControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the time at which to begin fading the haptic pattern.

### Audio Dynamic Parameter IDs

static let audioBrightnessControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the high-frequency content of an audio signal.

static let audioVolumeControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the volume or loudness of an audio signal.

static let audioPanControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the pan of an audio signal.

static let audioPitchControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the pitch of an audio signal.

static let audioAttackTimeControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the time when an audio signal’s amplitude begins increasing.

static let audioDecayTimeControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the time when an audio signal’s amplitude begins decreasing.

static let audioReleaseTimeControl: CHHapticDynamicParameter.ID

A dynamic parameter to change the time when an audio signal begins fading.

### Swift Initializers

init(rawValue: String)

Creates a dynamic property ID from its raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Dynamic Parameter

init(parameterID: CHHapticDynamicParameter.ID, value: Float, relativeTime: TimeInterval)

Creates a dynamic parameter from its ID, value, and start time.

