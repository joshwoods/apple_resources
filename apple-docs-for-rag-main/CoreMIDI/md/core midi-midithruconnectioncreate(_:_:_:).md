

- Core MIDI
-  MIDIThruConnectionCreate(\_:\_:\_:) 

Function

# MIDIThruConnectionCreate(\_:\_:\_:)

Creates a MIDI thru connection.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIThruConnectionCreate(
    _ inPersistentOwnerID: CFString?,
    _ inConnectionParams: CFData,
    _ outConnection: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inPersistentOwnerID`  

A unique identifier of the owning object, such as `com.mycompany.MyApp`. If you pass `NULL`, the client owns the connection and it’s automatically disposed with the client.

`inConnectionParams`  

A MIDIThruConnectionParams object that’s contained in a CFData.

`outConnection`  

On successful return, a reference to the newly created connection.

## Return Value

An `OSStatus` result code.

## See Also

### Managing Connections

func MIDIThruConnectionDispose(MIDIThruConnectionRef) -> OSStatus

Disposes a MIDI thru connection.

typealias MIDIThruConnectionRef

An opaque reference to a play-through connection.

struct MIDIThruConnectionEndpoint

A source or destination in a MIDI thru connection.

Endpoint Configuration

Values that define the supported endpoint configurations.

