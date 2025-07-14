

- Core MIDI
-  MIDICIResponder Deprecated

Class

# MIDICIResponder

An object that responds to MIDI-CI inquiries from an initiator on behalf of a MIDI client, and handles profile and property exchange operations.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class MIDICIResponder
```

Deprecated

No longer supported for CoreMIDI

## Topics

### Creating a Responder

init(deviceInfo: MIDICIDeviceInfo, profileDelegate: any MIDICIProfileResponderDelegate, profileStates: [MIDICIProfileState], supportProperties: Bool)

Creates a new responder.

### Managing the Life Cycle

func start() -> Bool

Starts receiving initiator requests.

func stop()

Stops receiving initiator requests and disconnects all connected initiators.

### Setting a Responder Delegate

var profileDelegate: any MIDICIProfileResponderDelegate

The profile delegate.

protocol MIDICIProfileResponderDelegate

A protocol that defines the methods to respond to MIDI-CI responder life-cycle events.

### Inspecting a Responder

typealias MIDICIInitiatiorMUID

The unique MIDI-CI negotiation identifier to use for a responder connection.

var initiators: [MIDICIInitiatiorMUID]

An array of initiators.

struct MIDICIDeviceIdentification

A structure that describes a MIDI-CI device.

class MIDICIDeviceInfo

An object that provides basic information about a MIDI-CI device.

var deviceInfo: MIDICIDeviceInfo

The MIDI-CI device’s information.

### Broadcasting Profile Changes

func notify(MIDICIProfile, onChannel: MIDIChannelNumber, isEnabled: Bool) -> Bool

Enables or disables a profile and notifies all connected initiators.

func send(MIDICIProfile, onChannel: MIDIChannelNumber, profileData: Data) -> Bool

Sends profile-specific data to all connected initiators.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

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

class MIDICIProfileState

An object that provides the enabled and disabled profiles for a MIDI channel or port on a device.

