

- Core MIDI
-  UnsafeMutableMIDIPacketPointer 

Structure

# UnsafeMutableMIDIPacketPointer

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+visionOS

``` source
struct UnsafeMutableMIDIPacketPointer
```

## Topics

### Initializers

init(UnsafeMutablePointer&lt;MIDIPacket>)

init?(UnsafeMutablePointer&lt;MIDIPacket>?)

### Instance Properties

var count: Int

var timeStamp: Int

### Default Implementations

MutableCollection Implementations

RandomAccessCollection Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- MutableCollection
- RandomAccessCollection
- Sequence

## See Also

### Packet list management

func MIDIPacketNext(UnsafePointer&lt;MIDIPacket>) -> UnsafeMutablePointer&lt;MIDIPacket>

Advances a MIDI packet pointer to the next packet in a package list.

struct MIDIPacket

A collection of simultaneous MIDI events.

struct MIDIPacketList

A list of MIDI events the system sends to or receives from an endpoint.

typealias MIDITimeStamp

The time on the host clock when the event occurred.

struct UnsafeMutableMIDIPacketListPointer

