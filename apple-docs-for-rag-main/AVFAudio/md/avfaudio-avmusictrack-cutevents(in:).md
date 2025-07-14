

- AVFAudio
- AVMusicTrack
-  cutEvents(in:) 

Instance Method

# cutEvents(in:)

Splices all events in the beat range from the music track.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func cutEvents(in range: AVBeatRange)
```

## Parameters 

`range`  

The range of beats.

## Discussion

All events past the end of the range you specify shift backward by the duration of the range.

## See Also

### Cutting and Copying Events

func copyEvents(in: AVBeatRange, from: AVMusicTrack, insertAt: AVMusicTimeStamp)

Copies the events from the source track and splices them into the current music track.

func copyAndMergeEvents(in: AVBeatRange, from: AVMusicTrack, mergeAt: AVMusicTimeStamp)

Copies the events from the source track and merges them into the current music track.

