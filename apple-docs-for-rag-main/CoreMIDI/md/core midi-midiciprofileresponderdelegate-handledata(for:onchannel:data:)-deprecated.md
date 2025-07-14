

- Core MIDI
- MIDICIProfileResponderDelegate
-  handleData(for:onChannel:data:) Deprecated

Instance Method

# handleData(for:onChannel:data:)

Processes MIDI data for a profile and channel.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
optional func handleData(
    for aProfile: MIDICIProfile,
    onChannel channel: MIDIChannelNumber,
    data inData: Data
)
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`aProfile`  

The MIDI-CI profile.

`channel`  

The MIDI channel.

`inData`  

The data to process.

## See Also

### Protocol Methods

func connectInitiator(MIDICIInitiatiorMUID, with: MIDICIDeviceInfo) -> Bool

Enables a MIDI-CI initiator to create a session or reject the connection attempt.

**Required**

Deprecated

func willSetProfile(MIDICIProfile, onChannel: MIDIChannelNumber, enabled: Bool) -> Bool

Provides an opportunity to perform an action before the system sets the profile.

Deprecated

func initiatorDisconnected(MIDICIInitiatiorMUID)

Provides an opportunity to perform an action after the system disconnects the initiator.

**Required**

Deprecated

