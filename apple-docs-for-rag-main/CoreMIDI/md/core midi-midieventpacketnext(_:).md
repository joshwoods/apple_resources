

- Core MIDI
-  MIDIEventPacketNext(\_:) 

Function

# MIDIEventPacketNext(\_:)

Advances a packet pointer to the next packet in memory, if the packet is part of an event list.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDIEventPacketNext(_ pkt: UnsafePointer) -> UnsafeMutablePointer
```

## Parameters 

`pkt`  

A pointer to a MIDIEventPacket in an event list.

## Return Value

The subsequent packet in the event list.

## See Also

### Event list management

func MIDIEventListInit(UnsafeMutablePointer&lt;MIDIEventList>, MIDIProtocolID) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Initializes an event list.

func MIDIEventListAdd(UnsafeMutablePointer&lt;MIDIEventList>, Int, UnsafeMutablePointer&lt;MIDIEventPacket>, MIDITimeStamp, Int, UnsafePointer&lt;UInt32>) -> UnsafeMutablePointer&lt;MIDIEventPacket>

Adds an event to an event list.

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

