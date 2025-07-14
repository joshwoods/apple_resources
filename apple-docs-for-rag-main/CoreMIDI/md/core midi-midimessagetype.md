

- Core MIDI
-  MIDIMessageType 

Enumeration

# MIDIMessageType

Supported MIDI message types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MIDIMessageType
```

## Topics

### Message Types

case channelVoice1

case channelVoice2

case data128

case sysEx

case system

case utility

### Enumeration Cases

case flexData

case invalid

case unknownF

### Initializers

init?(rawValue: UInt32)

### Type Properties

static var stream: MIDIMessageType

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
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

struct MIDIMessage_128

A 128-bit MIDI message.

struct MIDIMessage_96

A 96-bit MIDI message.

struct MIDIMessage_64

A 64-bit MIDI message.

typealias MIDIMessage_32

A 32-bit MIDI message.

