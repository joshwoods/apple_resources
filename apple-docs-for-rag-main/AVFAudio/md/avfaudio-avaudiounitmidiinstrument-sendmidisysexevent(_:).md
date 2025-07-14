

- AVFAudio
- AVAudioUnitMIDIInstrument
-  sendMIDISysExEvent(\_:) 

Instance Method

# sendMIDISysExEvent(\_:)

Sends a MIDI System Exclusive event to the instrument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func sendMIDISysExEvent(_ midiData: Data)
```

## Parameters 

`midiData`  

The system exclusive data you want to send to the instrument.

## Discussion

The `midiData` parameter should contain the complete `SysEx` data, including start (F0) and termination (F7) bytes.

## See Also

### Sending information to the MIDI instrument

func sendController(UInt8, withValue: UInt8, onChannel: UInt8)

Sends a MIDI controller event to the instrument.

func sendMIDIEvent(UInt8, data1: UInt8)

Sends a MIDI event which contains one data byte to the instrument.

func sendMIDIEvent(UInt8, data1: UInt8, data2: UInt8)

Sends a MIDI event which contains two data bytes to the instrument.

func sendPitchBend(UInt16, onChannel: UInt8)

Sends a MIDI Pitch Bend event to the instrument.

func sendPressure(UInt8, onChannel: UInt8)

Sends a MIDI channel pressure event to the instrument.

func sendPressure(forKey: UInt8, withValue: UInt8, onChannel: UInt8)

Sends a MIDI Polyphonic key pressure event to the instrument.

func sendProgramChange(UInt8, onChannel: UInt8)

Sends MIDI Program Change and Bank Select events to the instrument.

func sendProgramChange(UInt8, bankMSB: UInt8, bankLSB: UInt8, onChannel: UInt8)

Sends MIDI Program Change and Bank Select events to the instrument.

func send(UnsafePointer&lt;MIDIEventList>)

Sends a MIDI event list to the instrument.

