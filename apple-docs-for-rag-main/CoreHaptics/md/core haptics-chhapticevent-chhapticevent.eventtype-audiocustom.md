

- Core Haptics
- CHHapticEvent
- CHHapticEvent.EventType
-  audioCustom 

Type Property

# audioCustom

An audio event using a waveform that you supply.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let audioCustom: CHHapticEvent.EventType
```

## Discussion

Custom waveforms behave like transient events, with no looping.

## See Also

### Enumerating Haptic Types

static let audioContinuous: CHHapticEvent.EventType

An audio event with a looped waveform of arbitrary length.

static let hapticTransient: CHHapticEvent.EventType

A brief impulse occurring at a specific point in time, like the feedback from toggling a switch.

static let hapticContinuous: CHHapticEvent.EventType

A haptic event with a looped waveform of arbitrary length.

