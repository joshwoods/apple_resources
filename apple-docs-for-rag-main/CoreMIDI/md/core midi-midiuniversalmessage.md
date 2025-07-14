

- Core MIDI
-  MIDIUniversalMessage 

Structure

# MIDIUniversalMessage

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIUniversalMessage
```

## Topics

### Initializers

init()

### Instance Properties

var channelVoice1: MIDIUniversalMessage.__Unnamed_union___Anonymous_field3.__Unnamed_struct_channelVoice1

var channelVoice2: MIDIUniversalMessage.__Unnamed_union___Anonymous_field3.__Unnamed_struct_channelVoice2

var data128: MIDIUniversalMessage.__Unnamed_union___Anonymous_field3.__Unnamed_struct_data128

var group: UInt8

var reserved: (UInt8, UInt8, UInt8)

var sysEx: MIDIUniversalMessage.__Unnamed_union___Anonymous_field3.__Unnamed_struct_sysEx

var system: MIDIUniversalMessage.__Unnamed_union___Anonymous_field3.__Unnamed_struct_system

var type: MIDIMessageType

var unknown: MIDIUniversalMessage.__Unnamed_union___Anonymous_field3.__Unnamed_struct_unknown

var utility: MIDIUniversalMessage.__Unnamed_union___Anonymous_field3.__Unnamed_struct_utility

## Relationships

### Conforms To

- Sendable

## See Also

### Structures

struct MIDI2DeviceManufacturer

struct MIDI2DeviceRevisionLevel

struct MIDICIProfileID

struct MIDICIProfileIDManufacturerSpecific

struct MIDICIProfileIDStandard

