

- Core MIDI
- MIDICIProfileResponderDelegate
-  willSetProfile(\_:onChannel:enabled:) Deprecated

Instance Method

# willSetProfile(\_:onChannel:enabled:)

Provides an opportunity to perform an action before the system sets the profile.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
optional func willSetProfile(
    _ aProfile: MIDICIProfile,
    onChannel channel: MIDIChannelNumber,
    enabled shouldEnable: Bool
) -> Bool
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`aProfile`  

The profile the system uses to configure the device.

`channel`  

The MIDI channel assignment.

`shouldEnable`  

A Booean value that indicates whether the system should enable the profile.

## Return Value

A Boolean value that indicates whether the system enabled the profile.

## See Also

### Protocol Methods

func connectInitiator(MIDICIInitiatiorMUID, with: MIDICIDeviceInfo) -> Bool

Enables a MIDI-CI initiator to create a session or reject the connection attempt.

**Required**

Deprecated

func handleData(for: MIDICIProfile, onChannel: MIDIChannelNumber, data: Data)

Processes MIDI data for a profile and channel.

Deprecated

func initiatorDisconnected(MIDICIInitiatiorMUID)

Provides an opportunity to perform an action after the system disconnects the initiator.

**Required**

Deprecated

