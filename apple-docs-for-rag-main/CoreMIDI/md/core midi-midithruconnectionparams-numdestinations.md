

- Core MIDI
- MIDIThruConnectionParams
-  numDestinations 

Instance Property

# numDestinations

The number of valid destinations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var numDestinations: UInt32
```

## See Also

### Connection Parameters

var noteNumber: MIDITransform

The transformation of MIDI note numbers.

var lowNote: UInt8

The note value below which the system filters out notes.

var highNote: UInt8

The note value above which the system filters out notes.

var velocity: MIDITransform

A note velocity transformation.

var lowVelocity: UInt8

The velocity value below which the system filters out notes.

var highVelocity: UInt8

The velocity value above which the system filters out notes.

var keyPressure: MIDITransform

The transformation of polyphonic key pressure events.

var channelPressure: MIDITransform

The transformation of MIDI monophonic channel pressure events.

var version: UInt32

The version number.

var numSources: UInt32

The number of valid sources.

var sources: (MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint)

All MIDI sources for this connection.

var destinations: (MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint)

All MIDI destinations for this connection.

var channelMap: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

A mapping of MIDI channels.

var filterOutAllControls: UInt8

A value that indicates whether to filter out MIDI continuous control messages.

var filterOutBeatClock: UInt8

A value that indicates whether to filter out MIDI clock, play, stop, and resume messages.

