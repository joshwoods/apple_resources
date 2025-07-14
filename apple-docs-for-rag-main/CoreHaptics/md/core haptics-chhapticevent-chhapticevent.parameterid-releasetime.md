

- Core Haptics
- CHHapticEvent
- CHHapticEvent.ParameterID
-  releaseTime 

Type Property

# releaseTime

The time at which to begin fading the haptic pattern.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let releaseTime: CHHapticEvent.ParameterID
```

## Discussion

Specify the release time relative to the current time (`t = 0`), in seconds. It indicates when the pattern’s decay process begins. Its value ranges from `0` to `1`, with a default value of `0`.

## See Also

### Haptic Event Parameter IDs

static let hapticIntensity: CHHapticEvent.ParameterID

The strength of a haptic event.

static let hapticSharpness: CHHapticEvent.ParameterID

The feel of a haptic event.

static let attackTime: CHHapticEvent.ParameterID

The time at which a haptic pattern’s intensity begins increasing.

static let decayTime: CHHapticEvent.ParameterID

The time at which a haptic pattern’s intensity begins decreasing.

static let sustained: CHHapticEvent.ParameterID

A Boolean value that indicates whether to sustain a haptic event for its specified duration.

