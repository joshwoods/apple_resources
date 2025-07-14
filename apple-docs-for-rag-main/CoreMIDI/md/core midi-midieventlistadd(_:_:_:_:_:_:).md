

- Core MIDI
-  MIDIEventListAdd(\_:\_:\_:\_:\_:\_:) 

Function

# MIDIEventListAdd(\_:\_:\_:\_:\_:\_:)

Adds an event to an event list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func MIDIEventListAdd(
    _ evtlist: UnsafeMutablePointer,
    _ listSize: Int,
    _ curPacket: UnsafeMutablePointer,
    _ time: MIDITimeStamp,
    _ wordCount: Int,
    _ words: UnsafePointer
) -> UnsafeMutablePointer
```

## Parameters 

`evtlist`  

The event list to which to add the event.

`listSize`  

The event list’s capacity, in bytes.

`curPacket`  

A packet pointer returned by a previous call to MIDIEventListInit(_:_:) or MIDIEventListAdd(_:_:_:_:_:_:) for this packet list.

`time`  

The new event’s time.

`wordCount`  

The number of valid MIDI 32-bit words.

`words`  

The new event, which may be a single MIDI event or a partial SysEx event.

## Return Value

A packet pointer to pass as the `curPacket` argument in a subsequent call to this function, or `NULL` if there wasn’t room in the packet for the event.

## Discussion

The maximum size of an event list is 65,536 bytes. Send large SysEx messages in smaller event lists.

## See Also

### Event list management

func MIDIEventListInit(UnsafeMutablePointer&lt;MIDIEventList>, MIDIProtocolID) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Initializes an event list.

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

