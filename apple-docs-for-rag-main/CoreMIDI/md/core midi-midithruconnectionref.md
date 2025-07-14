

- Core MIDI
-  MIDIThruConnectionRef 

Type Alias

# MIDIThruConnectionRef

An opaque reference to a play-through connection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDIThruConnectionRef = MIDIObjectRef
```

## See Also

### Managing Connections

func MIDIThruConnectionCreate(CFString?, CFData, UnsafeMutablePointer&lt;MIDIThruConnectionRef>) -> OSStatus

Creates a MIDI thru connection.

func MIDIThruConnectionDispose(MIDIThruConnectionRef) -> OSStatus

Disposes a MIDI thru connection.

struct MIDIThruConnectionEndpoint

A source or destination in a MIDI thru connection.

Endpoint Configuration

Values that define the supported endpoint configurations.

