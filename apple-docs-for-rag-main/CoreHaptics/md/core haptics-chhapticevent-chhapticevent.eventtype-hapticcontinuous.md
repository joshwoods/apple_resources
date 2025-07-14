

- Core Haptics
- CHHapticEvent
- CHHapticEvent.EventType
-  hapticContinuous 

Type Property

# hapticContinuous

A haptic event with a looped waveform of arbitrary length.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let hapticContinuous: CHHapticEvent.EventType
```

## Discussion

Continuous haptic patterns, like the sustained vibration from a ringtone, take the form of lengthier feedback over a period of time. You must provide continuous events with a duration to determine their endpoint. The maximum duration of a continuous haptic event is 30 seconds.

## See Also

### Enumerating Haptic Types

static let audioContinuous: CHHapticEvent.EventType

An audio event with a looped waveform of arbitrary length.

static let audioCustom: CHHapticEvent.EventType

An audio event using a waveform that you supply.

static let hapticTransient: CHHapticEvent.EventType

A brief impulse occurring at a specific point in time, like the feedback from toggling a switch.

