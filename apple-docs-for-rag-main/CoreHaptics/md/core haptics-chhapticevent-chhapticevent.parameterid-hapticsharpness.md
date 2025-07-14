

- Core Haptics
- CHHapticEvent
- CHHapticEvent.ParameterID
-  hapticSharpness 

Type Property

# hapticSharpness

The feel of a haptic event.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let hapticSharpness: CHHapticEvent.ParameterID
```

## Discussion

Specify a pattern’s sharpness by setting this value from 0.0 to 1.0. Haptic patterns with low sharpness have a round and organic feel, whereas haptic patterns with high sharpness feel more crisp and precise. The diagram below depicts sharpness of haptic events as a single line to indicate the sensation of persistent feedback against the user’s hand:

To change the sharpness dynamically, use hapticSharpnessControl.

## See Also

### Haptic Event Parameter IDs

static let hapticIntensity: CHHapticEvent.ParameterID

The strength of a haptic event.

static let attackTime: CHHapticEvent.ParameterID

The time at which a haptic pattern’s intensity begins increasing.

static let decayTime: CHHapticEvent.ParameterID

The time at which a haptic pattern’s intensity begins decreasing.

static let releaseTime: CHHapticEvent.ParameterID

The time at which to begin fading the haptic pattern.

static let sustained: CHHapticEvent.ParameterID

A Boolean value that indicates whether to sustain a haptic event for its specified duration.

