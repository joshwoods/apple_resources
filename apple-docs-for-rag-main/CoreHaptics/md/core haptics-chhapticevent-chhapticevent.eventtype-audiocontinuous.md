

- Core Haptics
- CHHapticEvent
- CHHapticEvent.EventType
-  audioContinuous 

Type Property

# audioContinuous

An audio event with a looped waveform of arbitrary length.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let audioContinuous: CHHapticEvent.EventType
```

## Discussion

Continuous audio patterns take the form of lengthier feedback over a period of time. You must provide continuous events with a duration to determine their endpoint.

## See Also

### Enumerating Haptic Types

static let audioCustom: CHHapticEvent.EventType

An audio event using a waveform that you supply.

static let hapticTransient: CHHapticEvent.EventType

A brief impulse occurring at a specific point in time, like the feedback from toggling a switch.

static let hapticContinuous: CHHapticEvent.EventType

A haptic event with a looped waveform of arbitrary length.

