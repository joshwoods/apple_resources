

- Core Haptics
- CHHapticEvent
- CHHapticEvent.ParameterID
-  hapticIntensity 

Type Property

# hapticIntensity

The strength of a haptic event.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let hapticIntensity: CHHapticEvent.ParameterID
```

## Discussion

This parameter maps to the haptic pattern’s amplitude or strength. Its value ranges from 0.0 (weak) to 1.0 (strong). Think of intensity as the volume of a haptic pattern, indicating how impactful it feels in the user’s hand. The higher the haptic intensity, the stronger the resulting haptic.

To change the intensity dynamically, use hapticIntensityControl.

## See Also

### Haptic Event Parameter IDs

static let hapticSharpness: CHHapticEvent.ParameterID

The feel of a haptic event.

static let attackTime: CHHapticEvent.ParameterID

The time at which a haptic pattern’s intensity begins increasing.

static let decayTime: CHHapticEvent.ParameterID

The time at which a haptic pattern’s intensity begins decreasing.

static let releaseTime: CHHapticEvent.ParameterID

The time at which to begin fading the haptic pattern.

static let sustained: CHHapticEvent.ParameterID

A Boolean value that indicates whether to sustain a haptic event for its specified duration.

