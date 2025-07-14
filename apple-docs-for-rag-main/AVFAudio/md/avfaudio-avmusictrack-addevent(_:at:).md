

- AVFAudio
- AVMusicTrack
-  addEvent(\_:at:) 

Instance Method

# addEvent(\_:at:)

Adds a music event to a track at the time you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func addEvent(
    _ event: AVMusicEvent,
    at beat: AVMusicTimeStamp
)
```

## Parameters 

`event`  

The event to add.

`beat`  

The time to add the event at.

## Discussion

The system copies event contents into the track, so you can add the same event at different timestamps. You can’t add all AVMusicEvent subclasses to a track.

- You can only add AVExtendedTempoEvent and AVMIDIMetaEvent with certain AVMIDIMetaEvent.EventType to a sequencer’s tempo track.

- You can add AVParameterEvent to automation tracks.

- You can’t add other event subclasses to tempo or automation tracks.

## See Also

### Adding and Clearing Events

func moveEvents(in: AVBeatRange, by: AVMusicTimeStamp)

Moves the beat location of all events in the given beat range by the amount you specify.

func clearEvents(in: AVBeatRange)

Removes all events in the given beat range from the music track.

