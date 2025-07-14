

- Audio Toolbox
-  AUScheduleMIDIEventBlock 

Type Alias

# AUScheduleMIDIEventBlock

A block to schedule MIDI events.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUScheduleMIDIEventBlock = (AUEventSampleTime, UInt8, Int, UnsafePointer) -> Void
```

## Discussion

The block takes the following parameters:

eventSampleTime  
The sample time at which the MIDI event is to occur. When scheduling parameters during the render cycle, this time can be set to the `AUEventSampleTimeImmediate` value plus an optional buffer offset, in which case the event is scheduled at that position in the current render cycle.

cable  
The virtual cable number.

length  
The number of bytes of MIDI data in the provided event(s).

midiBytes  
One or more valid MIDI 1.0 events, except *sysex* which must always be sent as the only event in the chunk. Running status is not allowed.

## See Also

### Managing MIDI Events

var isMusicDeviceOrEffect: Bool

Specifies whether an audio unit responds to MIDI events.

var virtualMIDICableCount: Int

The number of virtual MIDI cables implemented by a music device or effect.

var scheduleMIDIEventBlock: AUScheduleMIDIEventBlock?

A block used to schedule MIDI events.

var midiOutputEventBlock: AUMIDIOutputEventBlock?

var midiOutputNames: [String]

The names of the MIDI outputs.

typealias AUMIDIOutputEventBlock

