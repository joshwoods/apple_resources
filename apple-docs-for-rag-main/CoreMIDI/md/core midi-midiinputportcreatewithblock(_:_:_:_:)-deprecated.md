

- Core MIDI
-  MIDIInputPortCreateWithBlock(\_:\_:\_:\_:) Deprecated

Function

# MIDIInputPortCreateWithBlock(\_:\_:\_:\_:)

Creates an input port through which the client may receive incoming MIDI messages from any MIDI source.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11–11.0DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func MIDIInputPortCreateWithBlock(
    _ client: MIDIClientRef,
    _ portName: CFString,
    _ outPort: UnsafeMutablePointer,
    _ readBlock: @escaping MIDIReadBlock
) -> OSStatus
```

Deprecated

Use MIDIInputPortCreateWithProtocol(_:_:_:_:_:) intead.

## Parameters 

`client`  

The client to own the newly-created port.

`portName`  

The name of the port.

`outPort`  

On successful return, points to the newly-created MIDIPort.

`readBlock`  

The MIDIReadBlock which will be called with incoming MIDI, from sources connected to this port.

## Return Value

An OSStatus result code.

## Discussion

After creating a port, use MIDIPortConnectSource to establish an input connection from any number of sources to your port.

readBlock will be called on a separate high-priority thread owned by CoreMIDI.

## See Also

### Deprecated Functions

func MIDIInputPortCreate(MIDIClientRef, CFString, MIDIReadProc, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;MIDIPortRef>) -> OSStatus

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

typealias MIDIReadBlock

A block receiving MIDI input.

Deprecated

