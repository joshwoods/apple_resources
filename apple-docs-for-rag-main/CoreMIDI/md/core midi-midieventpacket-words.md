

- Core MIDI
- MIDIEventPacket
-  words 

Instance Property

# words

A variable-length stream of native-endian 32-bit Universal MIDI Packets (UMP).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var words: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32)
```

## See Also

### Configuring an Event Packet

var timeStamp: MIDITimeStamp

The event packet timestamp.

var wordCount: UInt32

The number of valid MIDI 32-bit words in this event packet.

