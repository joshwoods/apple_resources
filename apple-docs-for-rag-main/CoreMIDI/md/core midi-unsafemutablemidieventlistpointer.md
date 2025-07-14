

- Core MIDI
-  UnsafeMutableMIDIEventListPointer 

Structure

# UnsafeMutableMIDIEventListPointer

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
struct UnsafeMutableMIDIEventListPointer
```

## Topics

### Initializers

init?(UnsafeMutablePointer&lt;MIDIEventList>?, wordSize: Int)

init(UnsafeMutablePointer&lt;MIDIEventList>, wordSize: Int, inProtocol: MIDIProtocolID)

### Instance Properties

var count: Int

var lastPacket: UnsafeMutablePointer&lt;MIDIEventPacket>?

var listSizeInBytes: Int

var midiProtocol: MIDIProtocolID

### Instance Methods

func append(timestamp: MIDITimeStamp, words: [UInt32]) -> UnsafePointer&lt;MIDIEventPacket>?

func clear()

## Relationships

### Conforms To

- Sequence

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

struct MIDIEventList

A variable-length list of MIDI event packets.

struct MIDIEventPacket

A series of simultaneous MIDI events in Universal MIDI Packets (UMP) format.

struct UnsafeMutableMIDIEventPacketPointer

