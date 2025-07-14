

- AVFAudio
- AVExtendedNoteOnEvent
-  instrumentID 

Instance Property

# instrumentID

The instrument identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var instrumentID: UInt32 { get set }
```

## Discussion

Set this value to defaultInstrument.

## See Also

### Configuring a Note On Event

var midiNote: Float

The MIDI note number.

var velocity: Float

The MDI velocity.

var groupID: UInt32

The audio unit channel that handles the event.

var duration: AVMusicTimeStamp

The duration of the event, in beats.

