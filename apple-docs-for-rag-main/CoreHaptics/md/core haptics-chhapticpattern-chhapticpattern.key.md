

- Core Haptics
- CHHapticPattern
-  CHHapticPattern.Key 

Structure

# CHHapticPattern.Key

Constants that define the keys you use to create a haptic pattern dictionary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
struct Key
```

## Topics

### Haptic Pattern Keys

static let event: CHHapticPattern.Key

A key that identifies the beginning of a haptic event definition.

static let eventDuration: CHHapticPattern.Key

A key that identifies the duration of an event.

static let eventParameters: CHHapticPattern.Key

A key that identifies the beginning of an array of fixed parameter definitions.

static let eventType: CHHapticPattern.Key

A key that identifies the type of event.

static let eventWaveformLoopEnabled: CHHapticPattern.Key

A key for a Boolean value that indicates whether to loop custom audio events.

static let eventWaveformPath: CHHapticPattern.Key

A key that identifies the path to the local file that contains the audio waveform.

static let eventWaveformUseVolumeEnvelope: CHHapticPattern.Key

A key that identifies whether audio file playback fades in and out using an envelope.

static let parameter: CHHapticPattern.Key

A key that identifies the beginning of a parameter definition.

static let parameterCurve: CHHapticPattern.Key

A key that identifies the beginning of a parameter curve definition.

static let parameterCurveControlPoints: CHHapticPattern.Key

A key that identifies the control points of a parameter curve.

static let parameterID: CHHapticPattern.Key

A key that identifies the parameter ID.

static let parameterValue: CHHapticPattern.Key

A key that identifies the value of a parameter.

static let pattern: CHHapticPattern.Key

A key that identifies the beginning of a haptic pattern definition.

static let time: CHHapticPattern.Key

A key that identifies the relative time for an event or parameter, in seconds.

static let version: CHHapticPattern.Key

A key that identifies rhe version number of a haptic pattern dictionary.

### Initializers

init(rawValue: String)

Creates a pattern key with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Haptic Pattern

init(contentsOf: URL) throws

Creates a haptic pattern with the contents of an AHAP file.

init(events: [CHHapticEvent], parameterCurves: [CHHapticParameterCurve]) throws

Constructs a haptic pattern from a series of events and parameter curves.

init(events: [CHHapticEvent], parameters: [CHHapticDynamicParameter]) throws

Constructs a haptic pattern from a series of events and parameters.

init(dictionary: [CHHapticPattern.Key : Any]) throws

Creates a haptic pattern from a property list dictionary.

