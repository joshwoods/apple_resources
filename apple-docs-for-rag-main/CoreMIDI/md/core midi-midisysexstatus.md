

- Core MIDI
-  MIDISysExStatus 

Enumeration

# MIDISysExStatus

MIDI System Exclusive (SysEx) types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MIDISysExStatus
```

## Topics

### Status Types

case complete

case start

case `continue`

case end

### Enumeration Cases

case mixedDataSetHeader

case mixedDataSetPayload

### Initializers

init?(rawValue: UInt32)

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

enum MIDIMessageType

Supported MIDI message types.

