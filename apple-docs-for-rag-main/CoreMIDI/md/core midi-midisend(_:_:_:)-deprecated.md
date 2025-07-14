

- Core MIDI
-  MIDISend(\_:\_:\_:) Deprecated

Function

# MIDISend(\_:\_:\_:)

Sends MIDI to a destination.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0–11.0DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func MIDISend(
    _ port: MIDIPortRef,
    _ dest: MIDIEndpointRef,
    _ pktlist: UnsafePointer
) -> OSStatus
```

Deprecated

Use MIDISendEventList(_:_:_:) instead.

## Parameters 

`port`  

The output port through which the MIDI is to be sent.

`dest`  

The destination to receive the events.

`pktlist`  

The MIDI events to be sent.

## Return Value

An OSStatus result code.

## Discussion

Events with future timestamps are scheduled for future delivery. CoreMIDI performs any needed MIDI merging.

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

func MIDIReceived(MIDIEndpointRef, UnsafePointer&lt;MIDIPacketList>) -> OSStatus

Distributes incoming MIDI from a source to the client input ports which are connected to that source.

Deprecated

typealias MIDIReadProc

A function receiving MIDI input.

Deprecated

typealias MIDIReadBlock

A block receiving MIDI input.

Deprecated

