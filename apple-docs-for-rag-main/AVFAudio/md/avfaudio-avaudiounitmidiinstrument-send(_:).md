

- AVFAudio
- AVAudioUnitMIDIInstrument
-  send(\_:) 

Instance Method

# send(\_:)

Sends a MIDI event list to the instrument.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func send(_ eventList: UnsafePointer)
```

## Parameters 

`eventList`  

The MIDI event list.

## See Also

### Sending information to the MIDI instrument

func sendController(UInt8, withValue: UInt8, onChannel: UInt8)

Sends a MIDI controller event to the instrument.

func sendMIDIEvent(UInt8, data1: UInt8)

Sends a MIDI event which contains one data byte to the instrument.

func sendMIDIEvent(UInt8, data1: UInt8, data2: UInt8)

Sends a MIDI event which contains two data bytes to the instrument.

func sendMIDISysExEvent(Data)

Sends a MIDI System Exclusive event to the instrument.

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

