

- Core MIDI
- MIDIPacket
-  MIDIPacket.ByteCollection 

Structure

# MIDIPacket.ByteCollection

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+visionOS

``` source
struct ByteCollection
```

## Topics

### Initializers

init(UnsafePointer&lt;MIDIPacket>)

init?(UnsafePointer&lt;MIDIPacket>?)

### Instance Properties

var count: Int

var endIndex: Int

var startIndex: Int

### Subscripts

subscript(MIDIPacket.ByteCollection.Index) -> MIDIPacket.ByteCollection.Element

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- RandomAccessCollection
- Sequence

