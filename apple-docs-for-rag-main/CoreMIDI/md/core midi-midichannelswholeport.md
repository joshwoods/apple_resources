

- Core MIDI
-  MIDIChannelsWholePort 

Global Variable

# MIDIChannelsWholePort

A constant value that indicates to use all channels of the port.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let MIDIChannelsWholePort: MIDIChannelNumber
```

## See Also

### Configuring a Session

func profileState(forChannel: MIDIChannelNumber) -> MIDICIProfileState

Returns the profile state for the specified MIDI channel number.

Deprecated

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

