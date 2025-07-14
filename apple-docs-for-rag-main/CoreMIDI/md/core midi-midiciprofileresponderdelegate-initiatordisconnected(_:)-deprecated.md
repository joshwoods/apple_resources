

- Core MIDI
- MIDICIProfileResponderDelegate
-  initiatorDisconnected(\_:) Deprecated

Instance Method

# initiatorDisconnected(\_:)

Provides an opportunity to perform an action after the system disconnects the initiator.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func initiatorDisconnected(_ initiatorMUID: MIDICIInitiatiorMUID)
```

**Required**

Deprecated

No longer supported for CoreMIDI

## Parameters 

`initiatorMUID`  

The MIDI-CI initiator identifier.

## See Also

### Protocol Methods

func connectInitiator(MIDICIInitiatiorMUID, with: MIDICIDeviceInfo) -> Bool

Enables a MIDI-CI initiator to create a session or reject the connection attempt.

**Required**

Deprecated

func handleData(for: MIDICIProfile, onChannel: MIDIChannelNumber, data: Data)

Processes MIDI data for a profile and channel.

Deprecated

func willSetProfile(MIDICIProfile, onChannel: MIDIChannelNumber, enabled: Bool) -> Bool

Provides an opportunity to perform an action before the system sets the profile.

Deprecated

