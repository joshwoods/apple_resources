

- AVFAudio
- AVAudioSequencer
-  beats(forHostTime:error:) 

Instance Method

# beats(forHostTime:error:)

Gets the beat the system plays at the specified host time.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func beats(
    forHostTime inHostTime: UInt64,
    error outError: NSErrorPointer
) -> AVMusicTimeStamp
```

## Parameters 

`inHostTime`  

The host time for the beat position.

`outError`  

On exit, if an error occurs, a description of the error.

## Discussion

This call is valid when the player is in a playing state. It returns `0` with an error, otherwise, or if the starting position of the player is after the specified host time. This method uses the sequence’s tempo map to retrieve a beat time from the specified host time.

## See Also

### Handling Beat Range

func beats(forSeconds: TimeInterval) -> AVMusicTimeStamp

Gets the beat position (timestamp) for the specified time in the track.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

typealias AVBeatRange

A specific time range within a music track.

