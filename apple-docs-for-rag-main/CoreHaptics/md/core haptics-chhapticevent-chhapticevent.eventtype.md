

- Core Haptics
- CHHapticEvent
-  CHHapticEvent.EventType 

Structure

# CHHapticEvent.EventType

The types of audio and haptic event waveforms.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
struct EventType
```

## Mentioned in 

Representing haptic patterns in AHAP files

## Topics

### Specifying a Type

init(rawValue: String)

Initializes an event type from a raw string value.

### Enumerating Haptic Types

static let audioContinuous: CHHapticEvent.EventType

An audio event with a looped waveform of arbitrary length.

static let audioCustom: CHHapticEvent.EventType

An audio event using a waveform that you supply.

static let hapticTransient: CHHapticEvent.EventType

A brief impulse occurring at a specific point in time, like the feedback from toggling a switch.

static let hapticContinuous: CHHapticEvent.EventType

A haptic event with a looped waveform of arbitrary length.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Categorizing Haptic Events

var type: CHHapticEvent.EventType

The type of the haptic event.

