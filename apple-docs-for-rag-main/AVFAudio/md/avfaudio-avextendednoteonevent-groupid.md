

- AVFAudio
- AVExtendedNoteOnEvent
-  groupID 

Instance Property

# groupID

The audio unit channel that handles the event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var groupID: UInt32 { get set }
```

## Discussion

The valid range of values are between `0` and `15`, but can be higher if the AVMusicTrack destination audio unit supports more channels.

## See Also

### Configuring a Note On Event

var midiNote: Float

The MIDI note number.

var velocity: Float

The MDI velocity.

var instrumentID: UInt32

The instrument identifier.

var duration: AVMusicTimeStamp

The duration of the event, in beats.

