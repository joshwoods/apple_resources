

- Core MIDI
-  MIDI2AssignablePNC(\_:\_:\_:\_:\_:) 

Function

# MIDI2AssignablePNC(\_:\_:\_:\_:\_:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDI2AssignablePNC(
    _ group: UInt8,
    _ channel: UInt8,
    _ noteNumber: UInt8,
    _ index: UInt8,
    _ value: UInt32
) -> MIDIMessage_64
```

## See Also

### MIDI 2.0 Messages

func MIDI2ChannelVoiceMessage(UInt8, UInt8, UInt8, UInt16, UInt32) -> MIDIMessage_64

func MIDI2NoteOn(UInt8, UInt8, UInt8, UInt8, UInt16, UInt16) -> MIDIMessage_64

func MIDI2NoteOff(UInt8, UInt8, UInt8, UInt8, UInt16, UInt16) -> MIDIMessage_64

func MIDI2ControlChange(UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2ProgramChange(UInt8, UInt8, Bool, UInt8, UInt8, UInt8) -> MIDIMessage_64

func MIDI2PitchBend(UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2PerNotePitchBend(UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2ChannelPressure(UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2PolyPressure(UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2AssignableControl(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2RelRegisteredControl(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2RegisteredPNC(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2RelAssignableControl(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2RegisteredControl(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2PerNoteManagment(UInt8, UInt8, UInt8, Bool, Bool) -> MIDIMessage_64

