

- Core MIDI
-  MIDIReceived(\_:\_:) Deprecated

Function

# MIDIReceived(\_:\_:)

Distributes incoming MIDI from a source to the client input ports which are connected to that source.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0–11.0DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func MIDIReceived(
    _ src: MIDIEndpointRef,
    _ pktlist: UnsafePointer
) -> OSStatus
```

Deprecated

Use MIDIReceivedEventList(_:_:) instead.

## Parameters 

`src`  

The source which is transmitting MIDI.

`pktlist`  

The MIDI events to be transmitted.

## Return Value

An OSStatus result code.

## Discussion

Drivers should call this function when receiving MIDI from a source.

Clients which have created virtual sources, using MIDISourceCreate, should call this function when the source is generating MIDI.

Unlike MIDISend(), a timestamp of 0 is not equivalent to “now”; the driver or virtual source is responsible for putting proper timestamps in the packets.

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

func MIDIPacketListAdd(UnsafeMutablePointer&lt;MIDIPacketList>, Int, UnsafeMutablePointer&lt;MIDIPacket>, MIDITimeStamp, Int, UnsafePointer&lt;UInt8>) -> UnsafeMutablePointer&lt;MIDIPacket>

Adds a MIDI event to a MIDIPacketList.

Deprecated

func MIDISend(MIDIPortRef, MIDIEndpointRef, UnsafePointer&lt;MIDIPacketList>) -> OSStatus

Sends MIDI to a destination.

Deprecated

typealias MIDIReadProc

A function receiving MIDI input.

Deprecated

typealias MIDIReadBlock

A block receiving MIDI input.

Deprecated

