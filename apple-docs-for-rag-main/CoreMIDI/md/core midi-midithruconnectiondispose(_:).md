

- Core MIDI
-  MIDIThruConnectionDispose(\_:) 

Function

# MIDIThruConnectionDispose(\_:)

Disposes a MIDI thru connection.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIThruConnectionDispose(_ connection: MIDIThruConnectionRef) -> OSStatus
```

## Parameters 

`connection`  

The connection to dispose.

## Return Value

An `OSStatus` result code.

## See Also

### Managing Connections

func MIDIThruConnectionCreate(CFString?, CFData, UnsafeMutablePointer&lt;MIDIThruConnectionRef>) -> OSStatus

Creates a MIDI thru connection.

typealias MIDIThruConnectionRef

An opaque reference to a play-through connection.

struct MIDIThruConnectionEndpoint

A source or destination in a MIDI thru connection.

Endpoint Configuration

Values that define the supported endpoint configurations.

