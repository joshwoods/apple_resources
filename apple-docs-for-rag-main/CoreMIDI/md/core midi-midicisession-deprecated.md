

- Core MIDI
-  MIDICISession Deprecated

Class

# MIDICISession

An object that represents a MIDI-CI session.

iOS 12.0–18.0DeprecatediPadOS 12.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class MIDICISession
```

Deprecated

No longer supported for CoreMIDI

## Overview

A MIDI-CI session is a bidirectional communication path between a MIDI source and destination identified using MIDI-CI discovery. Use a session to manipulate MIDI-CI profiles and to discover device capabilities.

## Topics

### Creating a Session

init(discoveredNode: MIDICIDiscoveredNode, dataReadyHandler: () -> Void, disconnectHandler: MIDICISessionDisconnectBlock)

Creates a MIDI-CI session.

### Configuring a Session

func profileState(forChannel: MIDIChannelNumber) -> MIDICIProfileState

Returns the profile state for the specified MIDI channel number.

func enable(MIDICIProfile, onChannel: MIDIChannelNumber) throws

Performs an asynchronous request to enable a profile for a specific MIDI channel number.

func disableProfile(MIDICIProfile, onChannel: MIDIChannelNumber) throws

Performs an asynchronous request to disable a profile for a specific MIDI channel number.

typealias MIDICIProfileChangedBlock

A block the system calls to indicate it has enabled or disabled a profile.

var profileChangedCallback: MIDICIProfileChangedBlock?

An optional block the system calls after it enables or disables a profile.

func send(MIDICIProfile, onChannel: MIDIChannelNumber, profileData: Data) -> Bool

Sends profile-specific data to the MIDI-CI session.

typealias MIDICIProfileSpecificDataBlock

A block the system calls when a MIDI-CI session or responder receives profile-specific data.

var profileSpecificDataHandler: MIDICIProfileSpecificDataBlock?

An optional block the system calls when a device sends profile-specific data to the session.

let MIDIChannelsWholePort: MIDIChannelNumber

A constant value that indicates to use all channels of the port.

### Inspecting a Session

var deviceInfo: MIDICIDeviceInfo

Information about a MIDI-CI device.

var maxSysExSize: NSNumber

The maximum size of System Exclusive (SysEx) messages.

var midiDestination: MIDIEntityRef

The MIDI destination with which the session is communicating.

var maxPropertyRequests: NSNumber

The maximum number of simultaneous property exchange requests, if supported.

var supportsProfileCapability: Bool

A Boolean value that indicates whether the entity supports the MIDI-CI profile’s capability.

var supportsPropertyCapability: Bool

A Boolean value that indicates whether the entity supports the MIDI-CI property exchange capability.

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

class MIDICIProfile

A mapping of MIDI messages to specific sounds and synthesis behaviors, such as General MIDI, a drawbar organ, and so on.

class MIDICIProfileState

An object that provides the enabled and disabled profiles for a MIDI channel or port on a device.

class MIDICIResponder

An object that responds to MIDI-CI inquiries from an initiator on behalf of a MIDI client, and handles profile and property exchange operations.

Deprecated

