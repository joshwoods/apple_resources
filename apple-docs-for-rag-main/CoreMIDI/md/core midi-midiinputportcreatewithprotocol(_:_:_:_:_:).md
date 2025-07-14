

- Core MIDI
-  MIDIInputPortCreateWithProtocol(\_:\_:\_:\_:\_:) 

Function

# MIDIInputPortCreateWithProtocol(\_:\_:\_:\_:\_:)

Creates an input port through which the client may receive incoming MIDI messages from any MIDI source.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func MIDIInputPortCreateWithProtocol(
    _ client: MIDIClientRef,
    _ portName: CFString,
    _ protocol: MIDIProtocolID,
    _ outPort: UnsafeMutablePointer,
    _ receiveBlock: @escaping MIDIReceiveBlock
) -> OSStatus
```

## Parameters 

`client`  

The client to own the newly created port.

`portName`  

The name of the port.

`protocol`  

The MIDI protocol variant to deliver to this port. The system automatically converts messages from one protocol to another as needed.

`outPort`  

On successful return, points to the newly created MIDI port.

`receiveBlock`  

A callback block the system invokes with incoming MIDI from sources connected to this port.

## Return Value

An `OSStatus` result code.

## Discussion

After creating a port, use MIDIPortConnectSource(_:_:_:) to establish an input connection from any number of sources to your port.

The system calls the receive block on a separate high-priority thread owned by Core MIDI.

## See Also

### Port management

func MIDIOutputPortCreate(MIDIClientRef, CFString, UnsafeMutablePointer&lt;MIDIPortRef>) -> OSStatus

Creates an output port through which a client sends outgoing MIDI messages to any MIDI destination.

func MIDIPortDispose(MIDIPortRef) -> OSStatus

Disposes of a MIDI port.

func MIDIPortConnectSource(MIDIPortRef, MIDIEndpointRef, UnsafeMutableRawPointer?) -> OSStatus

Makes a connection from a source to a client input port.

func MIDIPortDisconnectSource(MIDIPortRef, MIDIEndpointRef) -> OSStatus

Closes a previously established source-to-input port connection.

typealias MIDIPortRef

A MIDI connection that a client maintains.

typealias MIDIReceiveBlock

A block receiving MIDI input that includes the incoming messages and a refCon to identify the source.

