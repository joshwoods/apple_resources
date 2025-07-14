

- Core MIDI
-  MIDIMessage_128 

Structure

# MIDIMessage_128

A 128-bit MIDI message.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIMessage_128
```

## Topics

### Words

var word0: UInt32

var word1: UInt32

var word2: UInt32

var word3: UInt32

### Initializers

init()

init(word0: UInt32, word1: UInt32, word2: UInt32, word3: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Common

enum MIDICVStatus

MIDI status types.

enum MIDIProtocolID

Specifies a MIDI protocol variant.

enum MIDISysExStatus

MIDI System Exclusive (SysEx) types.

enum MIDISystemStatus

MIDI System status types.

struct MIDIMessage_96

A 96-bit MIDI message.

struct MIDIMessage_64

A 64-bit MIDI message.

typealias MIDIMessage_32

A 32-bit MIDI message.

enum MIDIMessageType

Supported MIDI message types.

