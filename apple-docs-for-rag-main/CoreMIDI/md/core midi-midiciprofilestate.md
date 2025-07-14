

- Core MIDI
-  MIDICIProfileState 

Class

# MIDICIProfileState

An object that provides the enabled and disabled profiles for a MIDI channel or port on a device.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
class MIDICIProfileState
```

## Topics

### Creating a Profile State

init(channel: MIDIChannelNumber, enabledProfiles: [MIDICIProfile], disabledProfiles: [MIDICIProfile])

Creates a new profile state object for the specified MIDI channel and profiles.

Deprecated

init(enabledProfiles: [MIDICIProfile], disabledProfiles: [MIDICIProfile])

Creates a new profile state object for the specified profiles.

Deprecated

### Accessing the MIDI Channel

var midiChannel: MIDIChannelNumber

The MIDI channel to which this state applies.

### Accessing Profiles

var enabledProfiles: [MIDICIProfile]

The object’s enabled profiles.

var disabledProfiles: [MIDICIProfile]

The object’s disabled profiles.

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

### Capability Inquiry

class MIDICIDiscoveryManager

A singleton object that performs systemwide MIDI-CI discovery.

Deprecated

class MIDICISession

An object that represents a MIDI-CI session.

Deprecated

class MIDICIProfile

A mapping of MIDI messages to specific sounds and synthesis behaviors, such as General MIDI, a drawbar organ, and so on.

class MIDICIResponder

An object that responds to MIDI-CI inquiries from an initiator on behalf of a MIDI client, and handles profile and property exchange operations.

Deprecated

