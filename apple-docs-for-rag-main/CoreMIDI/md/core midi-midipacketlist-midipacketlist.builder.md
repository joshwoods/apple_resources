

- Core MIDI
- MIDIPacketList
-  MIDIPacketList.Builder 

Class

# MIDIPacketList.Builder

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+visionOS

``` source
class Builder
```

## Topics

### Initializers

init(byteSize: Int)

### Instance Properties

var count: Int

### Instance Methods

func append(timestamp: MIDITimeStamp, data: [UInt8]) -> UnsafePointer&lt;MIDIPacket>?

func clear()

func withUnsafeMutableMIDIPacketListPointer&lt;Result>((inout UnsafeMutableMIDIPacketListPointer) -> Result) -> Result

func withUnsafePointer&lt;Result>((UnsafePointer&lt;MIDIPacketList>) -> Result) -> Result

