

- AVFAudio
- AVAudioSequencer
-  beats(forSeconds:) 

Instance Method

# beats(forSeconds:)

Gets the beat position (timestamp) for the specified time in the track.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func beats(forSeconds seconds: TimeInterval) -> AVMusicTimeStamp
```

## Parameters 

`seconds`  

The time to retrieve the beat timestamp for.

## See Also

### Handling Beat Range

func beats(forHostTime: UInt64, error: NSErrorPointer) -> AVMusicTimeStamp

Gets the beat the system plays at the specified host time.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

typealias AVBeatRange

A specific time range within a music track.

