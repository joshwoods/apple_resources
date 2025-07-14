

- Core MIDI
-  MIDIReadBlock Deprecated

Type Alias

# MIDIReadBlock

A block receiving MIDI input.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11–11.0DeprecatedvisionOS 1.0–2.4Deprecated

``` source
typealias MIDIReadBlock = (UnsafePointer, UnsafeMutableRawPointer?) -> Void
```

Deprecated

use MIDIReceiveBlock and MIDIEventLists

## Parameters 

`pktlist`  

The incoming MIDI message(s).

`srcConnRefCon`  

A refCon you passed to MIDIPortConnectSource, which identifies the source of the data.

## Discussion

This is a callback block through which a client receives incoming MIDI messages.

A MIDIReadBlock is passed to the MIDIInputPortCreateWithBlock and MIDIDestinationCreateWithBlock functions. The CoreMIDI framework will create a high-priority receive thread on your client’s behalf, and from that thread, your MIDIReadProc will be called when incoming MIDI messages arrive.

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

func MIDIReceived(MIDIEndpointRef, UnsafePointer&lt;MIDIPacketList>) -> OSStatus

Distributes incoming MIDI from a source to the client input ports which are connected to that source.

Deprecated

typealias MIDIReadProc

A function receiving MIDI input.

Deprecated

