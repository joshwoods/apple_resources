

- Core MIDI
- MIDI Thru Connection
-  Endpoint Configuration 

API Collection

# Endpoint Configuration

Values that define the supported endpoint configurations.

## Topics

### Configuration Constants

var kMIDIThruConnection_MaxEndpoints: Int

The maximum number of endpoints for this connection.

## See Also

### Managing Connections

func MIDIThruConnectionCreate(CFString?, CFData, UnsafeMutablePointer&lt;MIDIThruConnectionRef>) -> OSStatus

Creates a MIDI thru connection.

func MIDIThruConnectionDispose(MIDIThruConnectionRef) -> OSStatus

Disposes a MIDI thru connection.

typealias MIDIThruConnectionRef

An opaque reference to a play-through connection.

struct MIDIThruConnectionEndpoint

A source or destination in a MIDI thru connection.

