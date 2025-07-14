

- Core MIDI
- MIDIPacket
-  MIDIPacket.Builder 

Class

# MIDIPacket.Builder

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+visionOS

``` source
class Builder
```

## Topics

### Initializers

init(maximumNumberMIDIBytes: Int)

### Instance Properties

var capacity: Int

var count: Int

var timeStamp: Int

### Instance Methods

func append(UInt8...)

func withUnsafeMutableMIDIPacketPointer&lt;Result>((inout UnsafeMutableMIDIPacketPointer) -> Result) -> Result

func withUnsafePointer&lt;Result>((UnsafePointer&lt;MIDIPacket>) -> Result) -> Result

