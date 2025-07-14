

- Core MIDI
- MIDIEventPacket
-  MIDIEventPacket.Builder 

Class

# MIDIEventPacket.Builder

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
class Builder
```

## Topics

### Initializers

init(maximumNumberMIDIWords: Int)

### Instance Properties

var capacity: Int

var count: Int

var timeStamp: Int

### Instance Methods

func append(UInt32...)

func withUnsafeMutableMIDIEventPacketPointer&lt;Result>((inout UnsafeMutableMIDIEventPacketPointer) -> Result) -> Result

func withUnsafePointer&lt;Result>((UnsafePointer&lt;MIDIEventPacket>) -> Result) -> Result

