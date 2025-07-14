

- Core MIDI
-  MIDIEventList 

Structure

# MIDIEventList

A variable-length list of MIDI event packets.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIEventList
```

## Topics

### Configuring an Event List

var `protocol`: MIDIProtocolID

The MIDI protocol variant of the events in the list.

var numPackets: UInt32

The number of MIDI event packet structures in the list.

var packet: MIDIEventPacket

An array of variable-length MIDI event packet structures.

### Classes

class Builder

### Structures

struct UnsafeSequence

### Initializers

init()

init(protocol: MIDIProtocolID, numPackets: UInt32, packet: MIDIEventPacket)

### Type Methods

static func sizeInBytes(pktList: UnsafePointer&lt;MIDIEventList>) -> Int

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

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

func MIDIReceivedEventList(MIDIEndpointRef, UnsafePointer&lt;MIDIEventList>) -> OSStatus

Distributes incoming MIDI events from a source to its connected client input ports.

struct MIDIEventPacket

A series of simultaneous MIDI events in Universal MIDI Packets (UMP) format.

struct UnsafeMutableMIDIEventListPointer

struct UnsafeMutableMIDIEventPacketPointer

