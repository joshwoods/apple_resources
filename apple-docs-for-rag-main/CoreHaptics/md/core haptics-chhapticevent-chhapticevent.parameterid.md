

- Core Haptics
- CHHapticEvent
-  CHHapticEvent.ParameterID 

Structure

# CHHapticEvent.ParameterID

An identifier for an event parameter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
struct ParameterID
```

## Mentioned in 

Representing haptic patterns in AHAP files

## Discussion

Specify event parameters when creating a haptic or audio event. The combination of parameters determines the event’s character.

## Topics

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

static let sustained: CHHapticEvent.ParameterID

A Boolean value that indicates whether to sustain a haptic event for its specified duration.

### Audio Event Parameter IDs

static let audioVolume: CHHapticEvent.ParameterID

The volume of an audio event.

static let audioPan: CHHapticEvent.ParameterID

The stereo panning of an audio event.

static let audioPitch: CHHapticEvent.ParameterID

The pitch of an audio event.

static let audioBrightness: CHHapticEvent.ParameterID

The high-frequency content of an audio event.

### Swift Initializers

init(rawValue: String)

Creates the identifier of a haptic event parameter with the specified string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Haptic Events

var eventParameters: [CHHapticEventParameter]

An array of event parameters, possibly empty.

var relativeTime: TimeInterval

The start time of the event, relative to other events in the same pattern.

var duration: TimeInterval

The duration of the haptic event.

