

- Core Haptics
- CHHapticEvent
- CHHapticEvent.ParameterID
-  sustained 

Type Property

# sustained

A Boolean value that indicates whether to sustain a haptic event for its specified duration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let sustained: CHHapticEvent.ParameterID
```

## Discussion

This parameter is an event parameter. It determines whether or not the haptic continues playing at full strength after attack has finished, and before decay begins.

If true, the engine sustains the haptic pattern throughout its specified duration, increasing only during its attackTime, and decreasing only after its decayTime. If false, the haptic doesn’t stay at full strength between attack and decay, tailing off even before its decay has begun.

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

static let releaseTime: CHHapticEvent.ParameterID

The time at which to begin fading the haptic pattern.

