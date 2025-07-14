

- Core MIDI
-  MIDIGetSource(\_:) 

Function

# MIDIGetSource(\_:)

Returns a source in the system.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIGetSource(_ sourceIndex0: Int) -> MIDIEndpointRef
```

## Parameters 

`sourceIndex0`  

The source index.

## Return Value

A reference to a source, or `NULL` if an error occurred.

## See Also

### Endpoint management

func MIDIEndpointDispose(MIDIEndpointRef) -> OSStatus

Disposes of a virtual source or destination.

func MIDIEndpointGetEntity(MIDIEndpointRef, UnsafeMutablePointer&lt;MIDIEntityRef>?) -> OSStatus

Returns an endpoint’s entity.

func MIDIEndpointGetRefCons(MIDIEndpointRef, UnsafeMutablePointer&lt;UnsafeMutableRawPointer>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer>?) -> OSStatus

Returns contextual data assigned to an endpoint.

func MIDIEndpointSetRefCons(MIDIEndpointRef, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> OSStatus

Sets contextual data on an endpoint.

func MIDISourceCreateWithProtocol(MIDIClientRef, CFString, MIDIProtocolID, UnsafeMutablePointer&lt;MIDIEndpointRef>) -> OSStatus

Creates a virtual source in a client.

func MIDIGetNumberOfSources() -> Int

Returns the number of sources in the system.

func MIDIDestinationCreateWithProtocol(MIDIClientRef, CFString, MIDIProtocolID, UnsafeMutablePointer&lt;MIDIEndpointRef>, MIDIReceiveBlock) -> OSStatus

Creates a virtual destination in a client.

func MIDIGetDestination(Int) -> MIDIEndpointRef

Returns a destination in the system.

func MIDIGetNumberOfDestinations() -> Int

Returns the number of destinations in the system.

typealias MIDIEndpointRef

A MIDI source or destination an entity owns.

