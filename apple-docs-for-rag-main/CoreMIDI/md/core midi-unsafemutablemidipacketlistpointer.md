

- Core MIDI
-  UnsafeMutableMIDIPacketListPointer 

Structure

# UnsafeMutableMIDIPacketListPointer

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+visionOS

``` source
struct UnsafeMutableMIDIPacketListPointer
```

## Topics

### Initializers

init(UnsafeMutablePointer&lt;MIDIPacketList>, byteSize: Int)

init?(UnsafeMutablePointer&lt;MIDIPacketList>?, byteSize: Int)

### Instance Properties

var count: Int

var lastPacket: UnsafeMutablePointer&lt;MIDIPacket>?

var listSizeInBytes: Int

### Instance Methods

func append(timestamp: MIDITimeStamp, data: [UInt8]) -> UnsafePointer&lt;MIDIPacket>?

func clear()

## Relationships

### Conforms To

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

struct UnsafeMutableMIDIPacketPointer

