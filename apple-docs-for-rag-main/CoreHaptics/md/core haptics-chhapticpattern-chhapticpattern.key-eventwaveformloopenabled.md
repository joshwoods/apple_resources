

- Core Haptics
- CHHapticPattern
- CHHapticPattern.Key
-  eventWaveformLoopEnabled 

Type Property

# eventWaveformLoopEnabled

A key for a Boolean value that indicates whether to loop custom audio events.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
static let eventWaveformLoopEnabled: CHHapticPattern.Key
```

## Discussion

Set a value of true to indicate that events of type audioCustom should loop playback.

The default value is false.

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

