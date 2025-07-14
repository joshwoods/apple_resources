

- Core MIDI
-  MIDICIDeviceInfo Deprecated

Class

# MIDICIDeviceInfo

An object that provides basic information about a MIDI-CI device.

iOS 12.0–18.0DeprecatediPadOS 12.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class MIDICIDeviceInfo
```

Deprecated

No longer supported for CoreMIDI

## Topics

### Creating Device Information

init(destination: MIDIEntityRef, manufacturer: Data, family: Data, model: Data, revision: Data)

Creates a new device information instance.

### Inspecting a Device

var manufacturerID: Data

The MIDI System Exclusive (SysEx) ID of the device manufacturer.

var family: Data

The family to which the device belongs.

var modelNumber: Data

The model number of the device.

var revisionLevel: Data

The revision number of the device model number.

var midiDestination: MIDIEndpointRef

The MIDI destination the device’s MIDI entity uses for capability inquiries.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Inspecting a Responder

typealias MIDICIInitiatiorMUID

The unique MIDI-CI negotiation identifier to use for a responder connection.

var initiators: [MIDICIInitiatiorMUID]

An array of initiators.

Deprecated

struct MIDICIDeviceIdentification

A structure that describes a MIDI-CI device.

var deviceInfo: MIDICIDeviceInfo

The MIDI-CI device’s information.

Deprecated

