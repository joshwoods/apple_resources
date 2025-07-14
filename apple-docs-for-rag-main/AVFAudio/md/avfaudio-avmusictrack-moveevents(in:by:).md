

- AVFAudio
- AVMusicTrack
-  moveEvents(in:by:) 

Instance Method

# moveEvents(in:by:)

Moves the beat location of all events in the given beat range by the amount you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func moveEvents(
    in range: AVBeatRange,
    by beatAmount: AVMusicTimeStamp
)
```

## Parameters 

`range`  

The range of beats.

`beatAmount`  

The amount of beats to shift each event.

## See Also

### Adding and Clearing Events

func addEvent(AVMusicEvent, at: AVMusicTimeStamp)

Adds a music event to a track at the time you specify.

func clearEvents(in: AVBeatRange)

Removes all events in the given beat range from the music track.

