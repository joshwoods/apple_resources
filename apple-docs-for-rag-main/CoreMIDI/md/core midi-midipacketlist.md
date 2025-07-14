

- Core MIDI
-  MIDIPacketList 

Structure

# MIDIPacketList

A list of MIDI events the system sends to or receives from an endpoint.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIPacketList
```

## Topics

### Inspecting a Packet List

var numPackets: UInt32

The number of MIDI packets in the list.

var packet: MIDIPacket

An open-ended array of variable-length MIDI packets.

### Classes

class Builder

### Structures

struct UnsafeSequence

### Initializers

init()

init(numPackets: UInt32, packet: MIDIPacket)

### Type Methods

static func sizeInBytes(pktList: UnsafePointer&lt;MIDIPacketList>) -> Int

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Packet list management

func MIDIPacketNext(UnsafePointer&lt;MIDIPacket>) -> UnsafeMutablePointer&lt;MIDIPacket>

Advances a MIDI packet pointer to the next packet in a package list.

struct MIDIPacket

A collection of simultaneous MIDI events.

typealias MIDITimeStamp

The time on the host clock when the event occurred.

struct UnsafeMutableMIDIPacketListPointer

struct UnsafeMutableMIDIPacketPointer

