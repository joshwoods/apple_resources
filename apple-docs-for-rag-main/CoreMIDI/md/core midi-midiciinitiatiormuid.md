

- Core MIDI
-  MIDICIInitiatiorMUID 

Type Alias

# MIDICIInitiatiorMUID

The unique MIDI-CI negotiation identifier to use for a responder connection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDICIInitiatiorMUID = NSNumber
```

## Discussion

As required by the MIDI-CI specification, this value is a randomly assigned 28-bit integer.

## See Also

### Inspecting a Responder

var initiators: [MIDICIInitiatiorMUID]

An array of initiators.

Deprecated

struct MIDICIDeviceIdentification

A structure that describes a MIDI-CI device.

class MIDICIDeviceInfo

An object that provides basic information about a MIDI-CI device.

Deprecated

var deviceInfo: MIDICIDeviceInfo

The MIDI-CI device’s information.

Deprecated

