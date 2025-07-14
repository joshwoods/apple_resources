

- Core MIDI
-  MIDIPortDispose(\_:) 

Function

# MIDIPortDispose(\_:)

Disposes of a MIDI port.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIPortDispose(_ port: MIDIPortRef) -> OSStatus
```

## Parameters 

`port`  

The port to dispose of.

## Return Value

An `OSStatus` result code.

## Discussion

Calling this method explicitly isn’t required because the framework automatically disposes of clients at termination.

## See Also

### Port management

func MIDIInputPortCreateWithProtocol(MIDIClientRef, CFString, MIDIProtocolID, UnsafeMutablePointer&lt;MIDIPortRef>, MIDIReceiveBlock) -> OSStatus

Creates an input port through which the client may receive incoming MIDI messages from any MIDI source.

func MIDIOutputPortCreate(MIDIClientRef, CFString, UnsafeMutablePointer&lt;MIDIPortRef>) -> OSStatus

Creates an output port through which a client sends outgoing MIDI messages to any MIDI destination.

func MIDIPortConnectSource(MIDIPortRef, MIDIEndpointRef, UnsafeMutableRawPointer?) -> OSStatus

Makes a connection from a source to a client input port.

func MIDIPortDisconnectSource(MIDIPortRef, MIDIEndpointRef) -> OSStatus

Closes a previously established source-to-input port connection.

typealias MIDIPortRef

A MIDI connection that a client maintains.

typealias MIDIReceiveBlock

A block receiving MIDI input that includes the incoming messages and a refCon to identify the source.

