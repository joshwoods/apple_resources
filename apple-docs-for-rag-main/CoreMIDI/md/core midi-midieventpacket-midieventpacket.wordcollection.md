

- Core MIDI
- MIDIEventPacket
-  MIDIEventPacket.WordCollection 

Structure

# MIDIEventPacket.WordCollection

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
struct WordCollection
```

## Topics

### Initializers

init(UnsafePointer&lt;MIDIEventPacket>)

init?(UnsafePointer&lt;MIDIEventPacket>?)

### Instance Properties

var count: Int

var endIndex: Int

var startIndex: Int

### Subscripts

subscript(MIDIEventPacket.WordCollection.Index) -> MIDIEventPacket.WordCollection.Element

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- RandomAccessCollection
- Sequence

