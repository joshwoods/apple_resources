

- Core MIDI
-  MIDIObjectType 

Enumeration

# MIDIObjectType

The MIDI object types that the system supports.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MIDIObjectType
```

## Topics

### Object Types

case other

A MIDI object with an undefined type.

case device

A MIDI device.

case entity

A MIDI entity.

case source

A MIDI source.

case destination

A MIDI destination.

case externalDevice

An external device.

case externalEntity

An external entity.

case externalSource

An external source.

case externalDestination

An external destination.

let kMIDIObjectType_ExternalMask: MIDIObjectType

A bit mask indicating that a device is external.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Parameter Types

typealias MIDIUniqueID

A MIDI object’s unique identifier.

var kMIDIInvalidUniqueID: MIDIUniqueID

An invalid identifier.

