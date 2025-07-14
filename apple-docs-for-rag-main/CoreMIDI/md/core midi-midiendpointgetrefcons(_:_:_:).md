

- Core MIDI
-  MIDIEndpointGetRefCons(\_:\_:\_:) 

Function

# MIDIEndpointGetRefCons(\_:\_:\_:)

Returns contextual data assigned to an endpoint.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIEndpointGetRefCons(
    _ endpt: MIDIEndpointRef,
    _ ref1: UnsafeMutablePointer?,
    _ ref2: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`endpt`  

The endpoint with the `refCons` to return.

`ref1`  

On exit, the first `refCon`.

`ref2`  

On exit, the second `refCon`.

## Return Value

An OSStatus result code.

## See Also

### Endpoint management

func MIDIEndpointDispose(MIDIEndpointRef) -> OSStatus

Disposes of a virtual source or destination.

func MIDIEndpointGetEntity(MIDIEndpointRef, UnsafeMutablePointer&lt;MIDIEntityRef>?) -> OSStatus

Returns an endpoint’s entity.

func MIDIEndpointSetRefCons(MIDIEndpointRef, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> OSStatus

Sets contextual data on an endpoint.

func MIDISourceCreateWithProtocol(MIDIClientRef, CFString, MIDIProtocolID, UnsafeMutablePointer&lt;MIDIEndpointRef>) -> OSStatus

Creates a virtual source in a client.

func MIDIGetSource(Int) -> MIDIEndpointRef

Returns a source in the system.

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

