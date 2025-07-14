

- Core MIDI
-  MIDI1UPNoteOff(\_:\_:\_:\_:) 

Function

# MIDI1UPNoteOff(\_:\_:\_:\_:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDI1UPNoteOff(
    _ group: UInt8,
    _ channel: UInt8,
    _ noteNumber: UInt8,
    _ velocity: UInt8
) -> MIDIMessage_32
```

## See Also

### MIDI 1.0 Messages

func MIDI1UPNoteOn(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPPitchBend(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPControlChange(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPSystemCommon(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPChannelVoiceMessage(UInt8, UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDIMessageTypeForUPWord(UInt32) -> MIDIMessageType

