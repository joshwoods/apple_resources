

- Core MIDI
-  MIDICVStatus 

Enumeration

# MIDICVStatus

MIDI status types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MIDICVStatus
```

## Topics

### MIDI 1.0

case noteOff

case noteOn

case polyPressure

case controlChange

case programChange

case channelPressure

case pitchBend

### MIDI 2.0

case registeredPNC

case assignablePNC

case registeredControl

case assignableControl

case relRegisteredControl

case relAssignableControl

case perNotePitchBend

case perNoteMgmt

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

enum MIDIMessageType

Supported MIDI message types.

