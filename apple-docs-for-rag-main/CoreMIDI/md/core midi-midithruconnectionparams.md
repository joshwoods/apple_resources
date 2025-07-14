

- Core MIDI
-  MIDIThruConnectionParams 

Structure

# MIDIThruConnectionParams

A set of MIDI routings and transformations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIThruConnectionParams
```

## Topics

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

var numDestinations: UInt32

The number of valid destinations.

var destinations: (MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint)

All MIDI destinations for this connection.

var channelMap: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

A mapping of MIDI channels.

var filterOutAllControls: UInt8

A value that indicates whether to filter out MIDI continuous control messages.

var filterOutBeatClock: UInt8

A value that indicates whether to filter out MIDI clock, play, stop, and resume messages.

var filterOutMTC: UInt8

A value that indicates whether to filter out MIDI Time Code messages.

var filterOutSysEx: UInt8

A value that indicates wheter to filter out system-exclusive messages.

var filterOutTuneRequest: UInt8

A value that specifies whether to filter out MIDI tune request messages.

var numControlTransforms: UInt16

The number of control transformations in the variable-length portion of the struct.

var numMaps: UInt16

The number of MIDI value maps in the variable-length portion of the struct.

var pitchBend: MIDITransform

The transformation of a MIDI pitch bend event.

var programChange: MIDITransform

A transformation of a MIDI program change event.

var reserved2: (UInt8, UInt8, UInt8)

A reserved value that must be 0.

var reserved3: (UInt16, UInt16, UInt16, UInt16)

A reserved value that must be 0.

### Initializers

init()

init(version: UInt32, numSources: UInt32, sources: (MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint), numDestinations: UInt32, destinations: (MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint, MIDIThruConnectionEndpoint), channelMap: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8), lowVelocity: UInt8, highVelocity: UInt8, lowNote: UInt8, highNote: UInt8, noteNumber: MIDITransform, velocity: MIDITransform, keyPressure: MIDITransform, channelPressure: MIDITransform, programChange: MIDITransform, pitchBend: MIDITransform, filterOutSysEx: UInt8, filterOutMTC: UInt8, filterOutBeatClock: UInt8, filterOutTuneRequest: UInt8, reserved2: (UInt8, UInt8, UInt8), filterOutAllControls: UInt8, numControlTransforms: UInt16, numMaps: UInt16, reserved3: (UInt16, UInt16, UInt16, UInt16))

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Configuring Parameters

func MIDIThruConnectionParamsSize(UnsafePointer&lt;MIDIThruConnectionParams>) -> Int

Returns the size of a MIDI thru connection parameters object.

func MIDIThruConnectionParamsInitialize(UnsafeMutablePointer&lt;MIDIThruConnectionParams>)

Initializes a parameters object with its default values.

func MIDIThruConnectionGetParams(MIDIThruConnectionRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>>) -> OSStatus

Returns the thru connection’s parameters.

func MIDIThruConnectionSetParams(MIDIThruConnectionRef, CFData) -> OSStatus

Updates a thru connection’s parameters.

