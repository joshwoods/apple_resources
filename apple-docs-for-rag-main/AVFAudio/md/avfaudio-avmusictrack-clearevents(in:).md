

- AVFAudio
- AVMusicTrack
-  clearEvents(in:) 

Instance Method

# clearEvents(in:)

Removes all events in the given beat range from the music track.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func clearEvents(in range: AVBeatRange)
```

## Parameters 

`range`  

The range of beats.

## Discussion

The system won’t modify the events outside of the range you specify.

## See Also

### Adding and Clearing Events

func addEvent(AVMusicEvent, at: AVMusicTimeStamp)

Adds a music event to a track at the time you specify.

func moveEvents(in: AVBeatRange, by: AVMusicTimeStamp)

Moves the beat location of all events in the given beat range by the amount you specify.

