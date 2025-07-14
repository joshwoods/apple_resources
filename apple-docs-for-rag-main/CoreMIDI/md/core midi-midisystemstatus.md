

- Core MIDI
-  MIDISystemStatus 

Enumeration

# MIDISystemStatus

MIDI System status types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MIDISystemStatus
```

## Topics

### Status Types

case statusActiveSending

case statusContinue

case statusEndOfExclusive

case statusMTC

case statusSongPosPointer

case statusSongSelect

case statusStart

case statusStartOfExclusive

case statusStop

case statusSystemReset

case statusTimingClock

case statusTuneRequest

### Initializers

init?(rawValue: UInt32)

### Type Properties

static var statusActiveSensing: MIDISystemStatus

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

