

- Core MIDI
-  MIDICIProfile 

Class

# MIDICIProfile

A mapping of MIDI messages to specific sounds and synthesis behaviors, such as General MIDI, a drawbar organ, and so on.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
class MIDICIProfile
```

## Topics

### Creating a Profile

init(data: Data)

Creates a MIDI profile for the specified data.

init(data: Data, name: String)

Creates a named MIDI profile for the specified data.

### Inspecting a Profile

var name: String

A string that describes the profile.

var profileID: Data

The unique five-byte profile identifier that represents the profile.

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

class MIDICIProfileState

An object that provides the enabled and disabled profiles for a MIDI channel or port on a device.

class MIDICIResponder

An object that responds to MIDI-CI inquiries from an initiator on behalf of a MIDI client, and handles profile and property exchange operations.

Deprecated

