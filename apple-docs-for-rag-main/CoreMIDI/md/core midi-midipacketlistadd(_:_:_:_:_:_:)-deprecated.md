

- Core MIDI
-  MIDIPacketListAdd(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# MIDIPacketListAdd(\_:\_:\_:\_:\_:\_:)

Adds a MIDI event to a MIDIPacketList.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0–11.0DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func MIDIPacketListAdd(
    _ pktlist: UnsafeMutablePointer,
    _ listSize: Int,
    _ curPacket: UnsafeMutablePointer,
    _ time: MIDITimeStamp,
    _ nData: Int,
    _ data: UnsafePointer
) -> UnsafeMutablePointer
```

Deprecated

Use MIDIEventListAdd(_:_:_:_:_:_:) instead.

## Parameters 

`pktlist`  

The packet list to which the event is to be added.

`listSize`  

The size, in bytes, of the packet list.

`curPacket`  

A packet pointer returned by a previous call to MIDIPacketListInit or MIDIPacketListAdd for this packet list.

`time`  

The new event’s time.

`nData`  

The length of the new event, in bytes.

`data`  

The new event. May be a single MIDI event, or a partial sys-ex event. Running status is *not* permitted.

## Return Value

Returns null if there was not room in the packet for the event; otherwise returns a packet pointer which should be passed as curPacket in a subsequent call to this function.

## Discussion

The maximum size of a packet list is 65536 bytes. Large sysex messages must be sent in smaller packet lists.

## See Also

### Deprecated Functions

func MIDIInputPortCreate(MIDIClientRef, CFString, MIDIReadProc, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;MIDIPortRef>) -> OSStatus

Creates an input port through which the client may receive incoming MIDI messages from any MIDI source.

Deprecated

func MIDIInputPortCreateWithBlock(MIDIClientRef, CFString, UnsafeMutablePointer&lt;MIDIPortRef>, MIDIReadBlock) -> OSStatus

Creates an input port through which the client may receive incoming MIDI messages from any MIDI source.

Deprecated

func MIDISourceCreate(MIDIClientRef, CFString, UnsafeMutablePointer&lt;MIDIEndpointRef>) -> OSStatus

Creates a virtual source in a client.

Deprecated

func MIDIDestinationCreate(MIDIClientRef, CFString, MIDIReadProc, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;MIDIEndpointRef>) -> OSStatus

Creates a virtual destination in a client.

Deprecated

func MIDIDestinationCreateWithBlock(MIDIClientRef, CFString, UnsafeMutablePointer&lt;MIDIEndpointRef>, MIDIReadBlock) -> OSStatus

Creates a virtual destination in a client.

Deprecated

func MIDIPacketListInit(UnsafeMutablePointer&lt;MIDIPacketList>) -> UnsafeMutablePointer&lt;MIDIPacket>

Prepares a MIDIPacketList to be built up dynamically.

Deprecated

func MIDISend(MIDIPortRef, MIDIEndpointRef, UnsafePointer&lt;MIDIPacketList>) -> OSStatus

Sends MIDI to a destination.

Deprecated

func MIDIReceived(MIDIEndpointRef, UnsafePointer&lt;MIDIPacketList>) -> OSStatus

Distributes incoming MIDI from a source to the client input ports which are connected to that source.

Deprecated

typealias MIDIReadProc

A function receiving MIDI input.

Deprecated

typealias MIDIReadBlock

A block receiving MIDI input.

Deprecated

