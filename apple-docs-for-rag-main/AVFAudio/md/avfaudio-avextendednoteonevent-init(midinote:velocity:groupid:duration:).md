

- AVFAudio
- AVExtendedNoteOnEvent
-  init(midiNote:velocity:groupID:duration:) 

Initializer

# init(midiNote:velocity:groupID:duration:)

Creates an event with a MIDI note, velocity, group identifier, and duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    midiNote: Float,
    velocity: Float,
    groupID: UInt32,
    duration: AVMusicTimeStamp
)
```

## Parameters 

`midiNote`  

The MIDI note number.

`velocity`  

The MIDI velocity.

`groupID`  

The identifier that represents the audio unit channel that handles the event.

`duration`  

The duration of the event, in beats.

## See Also

### Creating a Note On Event

init(midiNote: Float, velocity: Float, instrumentID: UInt32, groupID: UInt32, duration: AVMusicTimeStamp)

Creates a note on event with the default instrument.

