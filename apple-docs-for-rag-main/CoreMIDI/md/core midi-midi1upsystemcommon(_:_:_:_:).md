

- Core MIDI
-  MIDI1UPSystemCommon(\_:\_:\_:\_:) 

Function

# MIDI1UPSystemCommon(\_:\_:\_:\_:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDI1UPSystemCommon(
    _ group: UInt8,
    _ status: UInt8,
    _ byte1: UInt8,
    _ byte2: UInt8
) -> MIDIMessage_32
```

## See Also

### MIDI 1.0 Messages

func MIDI1UPNoteOn(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPNoteOff(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPPitchBend(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPControlChange(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPChannelVoiceMessage(UInt8, UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDIMessageTypeForUPWord(UInt32) -> MIDIMessageType

