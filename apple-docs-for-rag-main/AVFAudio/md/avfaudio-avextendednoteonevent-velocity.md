

- AVFAudio
- AVExtendedNoteOnEvent
-  velocity 

Instance Property

# velocity

The MDI velocity.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var velocity: Float { get set }
```

## Discussion

If the instrument in the AVMusicTrack destination audio unit supports fractional values, use this to generate precise changes in gain and other values. The valid range of values depend on the destination audio unit, and is usually between `0.0` and `127.0`.

## See Also

### Configuring a Note On Event

var midiNote: Float

The MIDI note number.

var instrumentID: UInt32

The instrument identifier.

var groupID: UInt32

The audio unit channel that handles the event.

var duration: AVMusicTimeStamp

The duration of the event, in beats.

