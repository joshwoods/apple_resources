

- Core MIDI
- MIDICIResponder
-  send(\_:onChannel:profileData:) Deprecated

Instance Method

# send(\_:onChannel:profileData:)

Sends profile-specific data to all connected initiators.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func send(
    _ aProfile: MIDICIProfile,
    onChannel channel: MIDIChannelNumber,
    profileData profileSpecificData: Data
) -> Bool
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`aProfile`  

The profile to send.

`channel`  

The MIDI channel.

`profileSpecificData`  

The data to send.

## Return Value

A Boolean value that indicates whether the operation succeeded.

## See Also

### Broadcasting Profile Changes

func notify(MIDICIProfile, onChannel: MIDIChannelNumber, isEnabled: Bool) -> Bool

Enables or disables a profile and notifies all connected initiators.

Deprecated

