

- Core MIDI
-  MIDISendEventList(\_:\_:\_:) 

Function

# MIDISendEventList(\_:\_:\_:)

Sends MIDI events to a destination.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func MIDISendEventList(
    _ port: MIDIPortRef,
    _ dest: MIDIEndpointRef,
    _ evtlist: UnsafePointer
) -> OSStatus
```

## Parameters 

`port`  

The output port through which to send MIDI events.

`dest`  

The destination to receive the events.

`evtlist`  

The MIDI events to send.

## Return Value

An `OSStatus` result code.

## Discussion

The system schedules events with future timestamps for future delivery. It performs any needed MIDI merging.

## See Also

### Event list management

func MIDIEventListInit(UnsafeMutablePointer&lt;MIDIEventList>, MIDIProtocolID) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Initializes an event list.

func MIDIEventListAdd(UnsafeMutablePointer&lt;MIDIEventList>, Int, UnsafeMutablePointer&lt;MIDIEventPacket>, MIDITimeStamp, Int, UnsafePointer&lt;UInt32>) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Adds an event to an event list.

func MIDIEventPacketNext(UnsafePointer&lt;MIDIEventPacket>) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Advances a packet pointer to the next packet in memory, if the packet is part of an event list.

func MIDIReceivedEventList(MIDIEndpointRef, UnsafePointer&lt;MIDIEventList>) -> OSStatus

Distributes incoming MIDI events from a source to its connected client input ports.

struct MIDIEventList

A variable-length list of MIDI event packets.

struct MIDIEventPacket

A series of simultaneous MIDI events in Universal MIDI Packets (UMP) format.

struct UnsafeMutableMIDIEventListPointer

struct UnsafeMutableMIDIEventPacketPointer

