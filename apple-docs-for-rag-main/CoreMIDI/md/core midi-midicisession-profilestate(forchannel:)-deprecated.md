

- Core MIDI
- MIDICISession
-  profileState(forChannel:) Deprecated

Instance Method

# profileState(forChannel:)

Returns the profile state for the specified MIDI channel number.

iOS 12.0–18.0DeprecatediPadOS 12.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func profileState(forChannel channel: MIDIChannelNumber) -> MIDICIProfileState
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`channel`  

The MIDI channel for which you return the profile state.

## Return Value

A profile state object.

## See Also

### Configuring a Session

func enable(MIDICIProfile, onChannel: MIDIChannelNumber) throws

Performs an asynchronous request to enable a profile for a specific MIDI channel number.

Deprecated

func disableProfile(MIDICIProfile, onChannel: MIDIChannelNumber) throws

Performs an asynchronous request to disable a profile for a specific MIDI channel number.

Deprecated

typealias MIDICIProfileChangedBlock

A block the system calls to indicate it has enabled or disabled a profile.

Deprecated

var profileChangedCallback: MIDICIProfileChangedBlock?

An optional block the system calls after it enables or disables a profile.

Deprecated

func send(MIDICIProfile, onChannel: MIDIChannelNumber, profileData: Data) -> Bool

Sends profile-specific data to the MIDI-CI session.

Deprecated

typealias MIDICIProfileSpecificDataBlock

A block the system calls when a MIDI-CI session or responder receives profile-specific data.

Deprecated

var profileSpecificDataHandler: MIDICIProfileSpecificDataBlock?

An optional block the system calls when a device sends profile-specific data to the session.

Deprecated

let MIDIChannelsWholePort: MIDIChannelNumber

A constant value that indicates to use all channels of the port.

