

- Core MIDI
-  MIDIEventListInit(\_:\_:) 

Function

# MIDIEventListInit(\_:\_:)

Initializes an event list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func MIDIEventListInit(
    _ evtlist: UnsafeMutablePointer,
    _ protocol: MIDIProtocolID
) -> UnsafeMutablePointer
```

## Parameters 

`evtlist`  

The event list to initialize.

`protocol`  

The MIDI protocol variant.

## Return Value

A pointer to the first MIDIEventPacket in the event list.

## See Also

### Event list management

func MIDIEventListAdd(UnsafeMutablePointer&lt;MIDIEventList>, Int, UnsafeMutablePointer&lt;MIDIEventPacket>, MIDITimeStamp, Int, UnsafePointer&lt;UInt32>) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Adds an event to an event list.

func MIDIEventPacketNext(UnsafePointer&lt;MIDIEventPacket>) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Advances a packet pointer to the next packet in memory, if the packet is part of an event list.

func MIDISendEventList(MIDIPortRef, MIDIEndpointRef, UnsafePointer&lt;MIDIEventList>) -> OSStatus

Sends MIDI events to a destination.

func MIDIReceivedEventList(MIDIEndpointRef, UnsafePointer&lt;MIDIEventList>) -> OSStatus

Distributes incoming MIDI events from a source to its connected client input ports.

struct MIDIEventList

A variable-length list of MIDI event packets.

struct MIDIEventPacket

A series of simultaneous MIDI events in Universal MIDI Packets (UMP) format.

struct UnsafeMutableMIDIEventListPointer

struct UnsafeMutableMIDIEventPacketPointer

