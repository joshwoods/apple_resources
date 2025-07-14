

- Core MIDI
- MIDIEventList
-  MIDIEventList.Builder 

Class

# MIDIEventList.Builder

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
class Builder
```

## Topics

### Initializers

init(inProtocol: MIDIProtocolID, wordSize: Int)

### Instance Properties

var count: Int

### Instance Methods

func append(timestamp: MIDITimeStamp, words: [UInt32]) -> UnsafePointer&lt;MIDIEventPacket>?

func clear()

func withUnsafeMutableMIDIEventListPointer&lt;Result>((inout UnsafeMutableMIDIEventListPointer) -> Result) -> Result

func withUnsafePointer&lt;Result>((UnsafePointer&lt;MIDIEventList>) -> Result) -> Result

