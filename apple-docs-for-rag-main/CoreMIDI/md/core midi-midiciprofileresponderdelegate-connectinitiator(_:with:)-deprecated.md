

- Core MIDI
- MIDICIProfileResponderDelegate
-  connectInitiator(\_:with:) Deprecated

Instance Method

# connectInitiator(\_:with:)

Enables a MIDI-CI initiator to create a session or reject the connection attempt.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func connectInitiator(
    _ initiatorMUID: MIDICIInitiatiorMUID,
    with deviceInfo: MIDICIDeviceInfo
) -> Bool
```

**Required**

Deprecated

No longer supported for CoreMIDI

## Parameters 

`initiatorMUID`  

The ID of the MIDI-CI initiator.

`deviceInfo`  

The information that describes a device.

## See Also

### Protocol Methods

func handleData(for: MIDICIProfile, onChannel: MIDIChannelNumber, data: Data)

Processes MIDI data for a profile and channel.

Deprecated

func willSetProfile(MIDICIProfile, onChannel: MIDIChannelNumber, enabled: Bool) -> Bool

Provides an opportunity to perform an action before the system sets the profile.

Deprecated

func initiatorDisconnected(MIDICIInitiatiorMUID)

Provides an opportunity to perform an action after the system disconnects the initiator.

**Required**

Deprecated

