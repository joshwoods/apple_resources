

- Core MIDI
-  MIDIDestinationCreateWithProtocol(\_:\_:\_:\_:\_:) 

Function

# MIDIDestinationCreateWithProtocol(\_:\_:\_:\_:\_:)

Creates a virtual destination in a client.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func MIDIDestinationCreateWithProtocol(
    _ client: MIDIClientRef,
    _ name: CFString,
    _ protocol: MIDIProtocolID,
    _ outDest: UnsafeMutablePointer,
    _ readBlock: @escaping MIDIReceiveBlock
) -> OSStatus
```

## Parameters 

`client`  

The client that owns the virtual destination.

`name`  

The name of the virtual destination.

`protocol`  

The MIDI protocol variant to deliver to the destination. The system automatically converts messages to this protocol as needed.

`outDest`  

On successful return, a pointer to the newly created destination.

`readBlock`  

A callback block the system invokes when a client sends MIDI data to the virtual destination.

## Return Value

An `OSStatus` result code.

## Discussion

Drivers don’t need to call this function. When they create devices and entities, the system automatically creates sources and destinations at that time. See kMIDIPropertyAdvanceScheduleTimeMuSec for information about the relationship between when a sender sends MIDI data to the destination and when it’s received.

The system calls the read block on a separate high-priority thread owned by Core MIDI.

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

func MIDISourceCreateWithProtocol(MIDIClientRef, CFString, MIDIProtocolID, UnsafeMutablePointer&lt;MIDIEndpointRef>) -> OSStatus

Creates a virtual source in a client.

func MIDIGetSource(Int) -> MIDIEndpointRef

Returns a source in the system.

func MIDIGetNumberOfSources() -> Int

Returns the number of sources in the system.

func MIDIGetDestination(Int) -> MIDIEndpointRef

Returns a destination in the system.

func MIDIGetNumberOfDestinations() -> Int

Returns the number of destinations in the system.

typealias MIDIEndpointRef

A MIDI source or destination an entity owns.

