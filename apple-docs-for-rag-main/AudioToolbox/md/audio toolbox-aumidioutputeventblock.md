

- Audio Toolbox
-  AUMIDIOutputEventBlock 

Type Alias

# AUMIDIOutputEventBlock

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUMIDIOutputEventBlock = (AUEventSampleTime, UInt8, Int, UnsafePointer) -> OSStatus
```

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

typealias AUScheduleMIDIEventBlock

A block to schedule MIDI events.

