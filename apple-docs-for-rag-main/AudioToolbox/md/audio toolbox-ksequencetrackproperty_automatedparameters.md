

- Audio Toolbox
-  kSequenceTrackProperty_AutomatedParameters 

Global Variable

# kSequenceTrackProperty_AutomatedParameters

Indicates whether or not a music track’s purpose is audio unit parameter automation. If this property’s value is other than 0, music events in the track can only indicate points in an automation curve. A read/write `UInt32` value, where a value other than 0 indicates that the track is for parameter automation.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kSequenceTrackProperty_AutomatedParameters: UInt32 { get }
```

## See Also

### Constants

var kSequenceTrackProperty_LoopInfo: UInt32

Looping information for a music track.

var kSequenceTrackProperty_OffsetTime: UInt32

A music track’s start time in terms of beat number.

var kSequenceTrackProperty_MuteStatus: UInt32

The mute/unmute state of a music track. By default this value is `false` (not muted). A read/write Boolean value.

var kSequenceTrackProperty_SoloStatus: UInt32

The solo/unsolo state of a music track. By default this value is `false` (not soloed). A read/write Boolean value.

var kSequenceTrackProperty_TrackLength: UInt32

The time of the last music event in a music track, plus time required for note fade-outs and so on.

var kSequenceTrackProperty_TimeResolution: UInt32

The time resolution for a sequence of music events. For example, this value can indicate the time resolution that was specified by the MIDI file used to construct a sequence.

