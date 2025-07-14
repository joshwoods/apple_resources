

- AVFAudio
- AVMusicTrack
-  copyEvents(in:from:insertAt:) 

Instance Method

# copyEvents(in:from:insertAt:)

Copies the events from the source track and splices them into the current music track.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func copyEvents(
    in range: AVBeatRange,
    from sourceTrack: AVMusicTrack,
    insertAt insertStartBeat: AVMusicTimeStamp
)
```

## Parameters 

`range`  

The range of beats.

`sourceTrack`  

The music track to copy the events from.

`insertStartBeat`  

The start beat to splice the events into.

## Discussion

All events originally at or past the insertion beat shift forward by the duration of the copied-in range.

## See Also

### Cutting and Copying Events

func cutEvents(in: AVBeatRange)

Splices all events in the beat range from the music track.

func copyAndMergeEvents(in: AVBeatRange, from: AVMusicTrack, mergeAt: AVMusicTimeStamp)

Copies the events from the source track and merges them into the current music track.

