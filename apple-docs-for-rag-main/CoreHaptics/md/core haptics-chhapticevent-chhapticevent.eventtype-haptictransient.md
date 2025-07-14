

- Core Haptics
- CHHapticEvent
- CHHapticEvent.EventType
-  hapticTransient 

Type Property

# hapticTransient

A brief impulse occurring at a specific point in time, like the feedback from toggling a switch.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let hapticTransient: CHHapticEvent.EventType
```

## Mentioned in 

Playing a single-tap haptic pattern

## Discussion

Transient events complete on their own, even without a duration.

## See Also

### Enumerating Haptic Types

static let audioContinuous: CHHapticEvent.EventType

An audio event with a looped waveform of arbitrary length.

static let audioCustom: CHHapticEvent.EventType

An audio event using a waveform that you supply.

static let hapticContinuous: CHHapticEvent.EventType

A haptic event with a looped waveform of arbitrary length.

