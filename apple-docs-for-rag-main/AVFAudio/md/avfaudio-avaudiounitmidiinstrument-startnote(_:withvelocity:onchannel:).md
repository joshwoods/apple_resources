

- AVFAudio
- AVAudioUnitMIDIInstrument
-  startNote(\_:withVelocity:onChannel:) 

Instance Method

# startNote(\_:withVelocity:onChannel:)

Sends a MIDI Note On event to the instrument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func startNote(
    _ note: UInt8,
    withVelocity velocity: UInt8,
    onChannel channel: UInt8
)
```

## Parameters 

`note`  

The note number (key) to play. The valid range is `0` to `127`.

`velocity`  

Specifies the volume to play the note at. The valid range is `0` to `127`.

`channel`  

The channel number to send the event to. The valid range is `0` to `15`.

## See Also

### Starting and stopping play

func stopNote(UInt8, onChannel: UInt8)

Sends a MIDI Note Off event to the instrument.

