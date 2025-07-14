

- Core MIDI
-  MIDIPortDisconnectSource(\_:\_:) 

Function

# MIDIPortDisconnectSource(\_:\_:)

Closes a previously established source-to-input port connection.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIPortDisconnectSource(
    _ port: MIDIPortRef,
    _ source: MIDIEndpointRef
) -> OSStatus
```

## Parameters 

`port`  

The port with the connection to close.

`source`  

The source from which to close a connection to a port.

## Return Value

An `OSStatus` result code.

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

typealias MIDIPortRef

A MIDI connection that a client maintains.

typealias MIDIReceiveBlock

A block receiving MIDI input that includes the incoming messages and a refCon to identify the source.

