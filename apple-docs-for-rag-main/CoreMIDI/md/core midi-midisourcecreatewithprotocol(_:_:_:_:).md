

- Core MIDI
-  MIDISourceCreateWithProtocol(\_:\_:\_:\_:) 

Function

# MIDISourceCreateWithProtocol(\_:\_:\_:\_:)

Creates a virtual source in a client.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func MIDISourceCreateWithProtocol(
    _ client: MIDIClientRef,
    _ name: CFString,
    _ protocol: MIDIProtocolID,
    _ outSrc: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`client`  

The client to own the virtual source.

`name`  

The name of the virtual source.

`protocol`  

The MIDI protocol variant to send from this source. The system automatically converts messages from this protocol to the protocol of the destination.

`outSrc`  

On successful return, a pointer to the newly created source.

## Return Value

An `OSStatus` result code.

## Discussion

Drivers don’t need to call this function. When they create devices and entities, the system automatically creates sources and destinations at that time. After creating a virtual source, use MIDIReceivedEventList(_:_:) to transmit MIDI messages from your virtual source to any clients connected to the virtual source.

Tip

After creating a virtual source, assign it the same unique ID it had the last time your app created it. Doing so permits other clients to retain persistent references to your virtual source.

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

