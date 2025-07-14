

- Core MIDI
-  MIDICIDeviceIdentification 

Structure

# MIDICIDeviceIdentification

A structure that describes a MIDI-CI device.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDICIDeviceIdentification
```

## Topics

### Configuring Device Identification

var manufacturer: (UInt8, UInt8, UInt8)

The MIDI System Exclusive (SysEx) ID of the device manufacturer.

var modelNumber: (UInt8, UInt8)

The device model number.

var family: (UInt8, UInt8)

The group of familes to which the device belongs.

var revisionLevel: (UInt8, UInt8, UInt8, UInt8)

The revision number of the device model number.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8)

A reserved field whose value is always zero.

### Initializers

init()

init(manufacturer: (UInt8, UInt8, UInt8), family: (UInt8, UInt8), modelNumber: (UInt8, UInt8), revisionLevel: (UInt8, UInt8, UInt8, UInt8), reserved: (UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Inspecting a Responder

typealias MIDICIInitiatiorMUID

The unique MIDI-CI negotiation identifier to use for a responder connection.

var initiators: [MIDICIInitiatiorMUID]

An array of initiators.

Deprecated

class MIDICIDeviceInfo

An object that provides basic information about a MIDI-CI device.

Deprecated

var deviceInfo: MIDICIDeviceInfo

The MIDI-CI device’s information.

Deprecated

