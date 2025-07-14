

- Core MIDI
-  MIDIEndpointGetEntity(\_:\_:) 

Function

# MIDIEndpointGetEntity(\_:\_:)

Returns an endpoint’s entity.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIEndpointGetEntity(
    _ inEndpoint: MIDIEndpointRef,
    _ outEntity: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inEndpoint`  

The endpoint to query.

`outEntity`  

On exit, the endpoint’s owning entity, or `NULL` if none.

## Return Value

An `OSStatus` result code.

## Discussion

Virtual sources and destinations don’t have entities.

## See Also

### Endpoint management

func MIDIEndpointDispose(MIDIEndpointRef) -> OSStatus

Disposes of a virtual source or destination.

func MIDIEndpointGetRefCons(MIDIEndpointRef, UnsafeMutablePointer&lt;UnsafeMutableRawPointer>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer>?) -> OSStatus

Returns contextual data assigned to an endpoint.

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

