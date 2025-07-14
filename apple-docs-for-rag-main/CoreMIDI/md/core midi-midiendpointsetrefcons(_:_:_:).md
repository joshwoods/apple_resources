

- Core MIDI
-  MIDIEndpointSetRefCons(\_:\_:\_:) 

Function

# MIDIEndpointSetRefCons(\_:\_:\_:)

Sets contextual data on an endpoint.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIEndpointSetRefCons(
    _ endpt: MIDIEndpointRef,
    _ ref1: UnsafeMutableRawPointer?,
    _ ref2: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`endpt`  

The endpoint to set the data on.

`ref1`  

The first `refCon`.

`ref2`  

The second `refCon`.

## Return Value

An OSStatus result code.

## Discussion

Drivers need an efficient way to translate from a MIDIEndpointRef (source or destination) to their own internal data structures corresponding to that endpoint. This function provides a way for the driver to assign its own data to endpoints.

The data you set isn’t persistent and needs to be reintialized in each call to Start.

A typical use is for one `refCon` to refer to a device, and a second to refer to a port on the device.

## See Also

### Endpoint management

func MIDIEndpointDispose(MIDIEndpointRef) -> OSStatus

Disposes of a virtual source or destination.

func MIDIEndpointGetEntity(MIDIEndpointRef, UnsafeMutablePointer&lt;MIDIEntityRef>?) -> OSStatus

Returns an endpoint’s entity.

func MIDIEndpointGetRefCons(MIDIEndpointRef, UnsafeMutablePointer&lt;UnsafeMutableRawPointer>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer>?) -> OSStatus

Returns contextual data assigned to an endpoint.

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

