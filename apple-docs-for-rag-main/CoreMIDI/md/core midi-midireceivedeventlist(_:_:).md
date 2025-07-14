

- Core MIDI
-  MIDIReceivedEventList(\_:\_:) 

Function

# MIDIReceivedEventList(\_:\_:)

Distributes incoming MIDI events from a source to its connected client input ports.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func MIDIReceivedEventList(
    _ src: MIDIEndpointRef,
    _ evtlist: UnsafePointer
) -> OSStatus
```

## Parameters 

`src`  

The source that’s transmitting MIDI events.

`evtlist`  

The MIDI events to transmit.

## Return Value

An `OSStatus` result code.

## Discussion

Drivers can call this function when receiving MIDI events from a source.

Clients that create virtual sources, using MIDISourceCreateWithProtocol(_:_:_:_:), can call this function when the source is generating MIDI events.

## See Also

### Event list management

func MIDIEventListInit(UnsafeMutablePointer&lt;MIDIEventList>, MIDIProtocolID) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Initializes an event list.

func MIDIEventListAdd(UnsafeMutablePointer&lt;MIDIEventList>, Int, UnsafeMutablePointer&lt;MIDIEventPacket>, MIDITimeStamp, Int, UnsafePointer&lt;UInt32>) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Adds an event to an event list.

func MIDIEventPacketNext(UnsafePointer&lt;MIDIEventPacket>) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Advances a packet pointer to the next packet in memory, if the packet is part of an event list.

func MIDISendEventList(MIDIPortRef, MIDIEndpointRef, UnsafePointer&lt;MIDIEventList>) -> OSStatus

Sends MIDI events to a destination.

struct MIDIEventList

A variable-length list of MIDI event packets.

struct MIDIEventPacket

A series of simultaneous MIDI events in Universal MIDI Packets (UMP) format.

struct UnsafeMutableMIDIEventListPointer

struct UnsafeMutableMIDIEventPacketPointer

