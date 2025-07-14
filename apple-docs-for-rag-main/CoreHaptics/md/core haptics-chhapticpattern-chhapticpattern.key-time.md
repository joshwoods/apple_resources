

- Core Haptics
- CHHapticPattern
- CHHapticPattern.Key
-  time 

Type Property

# time

A key that identifies the relative time for an event or parameter, in seconds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let time: CHHapticPattern.Key
```

## Discussion

The value associated with the key is a real number in units of seconds.

## See Also

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

static let version: CHHapticPattern.Key

A key that identifies rhe version number of a haptic pattern dictionary.

