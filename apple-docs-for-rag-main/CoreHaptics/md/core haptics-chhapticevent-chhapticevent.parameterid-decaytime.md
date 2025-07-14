

- Core Haptics
- CHHapticEvent
- CHHapticEvent.ParameterID
-  decayTime 

Type Property

# decayTime

The time at which a haptic pattern’s intensity begins decreasing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let decayTime: CHHapticEvent.ParameterID
```

## Discussion

This parameter can be an event parameter or a dynamic parameter. A fixed value indicates that the haptic begins decreasing in intensity at the set time, where time `0` indicates now, or the current time.

A dynamic value indicates that the start time of the decrease can change. For example, a value of `0` indicates that the decay time is at its default value. Positive values up to `1.0` increase the decay time exponentially, while negative values down to `-1.0` decrease the decay time exponentially.

Haptic intensity responds to this parameter. For example, the following graphic shows the intensity of a haptic pattern in gray. At the beginning, the haptic pattern’s intensity increases from zero to its final value over a certain amount of time; this duration is called the *attack*. As the haptic pattern reaches its end, the intensity gradually transitions to zero over a certain amount of time; this duration is called the *decay*.

## See Also

### Haptic Event Parameter IDs

static let hapticIntensity: CHHapticEvent.ParameterID

The strength of a haptic event.

static let hapticSharpness: CHHapticEvent.ParameterID

The feel of a haptic event.

static let attackTime: CHHapticEvent.ParameterID

The time at which a haptic pattern’s intensity begins increasing.

static let releaseTime: CHHapticEvent.ParameterID

The time at which to begin fading the haptic pattern.

static let sustained: CHHapticEvent.ParameterID

A Boolean value that indicates whether to sustain a haptic event for its specified duration.

