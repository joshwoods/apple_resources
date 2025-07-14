

- AVFAudio
- AVExtendedNoteOnEvent
-  midiNote 

Instance Property

# midiNote

The MIDI note number.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var midiNote: Float { get set }
```

## Discussion

If the instrument within the AVMusicTrack destination audio unit supports fractional values, you use this to generate arbitrary tunings. The valid range of values depends on the destination audio unit, and is usually between `0.0` and `127.0`.

## See Also

### Configuring a Note On Event

var velocity: Float

The MDI velocity.

var instrumentID: UInt32

The instrument identifier.

var groupID: UInt32

The audio unit channel that handles the event.

var duration: AVMusicTimeStamp

The duration of the event, in beats.

