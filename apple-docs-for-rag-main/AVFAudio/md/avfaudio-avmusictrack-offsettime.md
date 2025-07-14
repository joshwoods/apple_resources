

- AVFAudio
- AVMusicTrack
-  offsetTime 

Instance Property

# offsetTime

The offset of the track’s start time, in beats.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var offsetTime: AVMusicTimeStamp { get set }
```

## Discussion

By default, this value is `0`.

## See Also

### Configuring Music Track Properties

var isMuted: Bool

A Boolean value that indicates whether the track is in a muted state.

var isSoloed: Bool

A Boolean value that indicates whether the track is in a soloed state.

var timeResolution: Int

The time resolution value for the sequence, in ticks (pulses) per quarter note.

var usesAutomatedParameters: Bool

A Boolean value that indicates whether the track is an automation track.

