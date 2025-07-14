

- Core MIDI
-  MIDIReceiveBlock 

Type Alias

# MIDIReceiveBlock

A block receiving MIDI input that includes the incoming messages and a refCon to identify the source.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDIReceiveBlock = (UnsafePointer, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`evtlist`  

The incoming MIDI message(s).

`srcConnRefCon`  

The refCon that identifies the source of the data, which is the value that you pass for the `connRefCon` parameter to MIDIPortConnectSource(_:_:_:). This value is always nil when receiving a MIDI event on a virtual input.

## Discussion

A client receives incoming MIDI messages through this callback block.

The MIDIInputPortCreateWithProtocol(_:_:_:_:_:) and MIDIDestinationCreateWithProtocol(_:_:_:_:_:) functions receive a MIDIReceiveBlock. The system creates a high-priority receive thread on your client’s behalf, and from that thread it calls your MIDIReceiveBlock when incoming MIDI messages arrive.

## See Also

### Port management

func MIDIInputPortCreateWithProtocol(MIDIClientRef, CFString, MIDIProtocolID, UnsafeMutablePointer&lt;MIDIPortRef>, MIDIReceiveBlock) -> OSStatus

Creates an input port through which the client may receive incoming MIDI messages from any MIDI source.

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

