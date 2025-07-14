

- Core MIDI
-  MIDI1UPChannelVoiceMessage(\_:\_:\_:\_:\_:) 

Function

# MIDI1UPChannelVoiceMessage(\_:\_:\_:\_:\_:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDI1UPChannelVoiceMessage(
    _ group: UInt8,
    _ status: UInt8,
    _ channel: UInt8,
    _ data1: UInt8,
    _ data2: UInt8
) -> MIDIMessage_32
```

## See Also

### MIDI 1.0 Messages

func MIDI1UPNoteOn(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPNoteOff(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPPitchBend(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPControlChange(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPSystemCommon(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDIMessageTypeForUPWord(UInt32) -> MIDIMessageType

