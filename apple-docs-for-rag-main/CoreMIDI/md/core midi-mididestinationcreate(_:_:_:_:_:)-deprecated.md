

- Core MIDI
-  MIDIDestinationCreate(\_:\_:\_:\_:\_:) Deprecated

Function

# MIDIDestinationCreate(\_:\_:\_:\_:\_:)

Creates a virtual destination in a client.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0–11.0DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func MIDIDestinationCreate(
    _ client: MIDIClientRef,
    _ name: CFString,
    _ readProc: MIDIReadProc,
    _ refCon: UnsafeMutableRawPointer?,
    _ outDest: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

Use MIDIDestinationCreateWithProtocol(_:_:_:_:_:) instead.

## Parameters 

`client`  

The client owning the virtual destination.

`name`  

The name of the virtual destination.

`readProc`  

The MIDIReadProc to be called when a client sends MIDI to the virtual destination.

`refCon`  

The refCon to be passed to the readProc.

`outDest`  

On successful return, a pointer to the newly-created destination.

## Return Value

An OSStatus result code.

## Discussion

The specified readProc gets called when clients send MIDI to your virtual destination.

Drivers need not call this; when they create devices and entities, sources and destinations are created at that time.

After creating a virtual destination, it’s a good idea to assign it the same unique ID it had the last time your application created it. (Although you should be prepared for this to fail in the unlikely event of a collision.) This will permit other clients to retain persistent references to your virtual destination more easily.

See the discussion of kMIDIPropertyAdvanceScheduleTimeMuSec for notes about the relationship between when a sender sends MIDI to the destination and when it is received.

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

func MIDIReceived(MIDIEndpointRef, UnsafePointer&lt;MIDIPacketList>) -> OSStatus

Distributes incoming MIDI from a source to the client input ports which are connected to that source.

Deprecated

typealias MIDIReadProc

A function receiving MIDI input.

Deprecated

typealias MIDIReadBlock

A block receiving MIDI input.

Deprecated

