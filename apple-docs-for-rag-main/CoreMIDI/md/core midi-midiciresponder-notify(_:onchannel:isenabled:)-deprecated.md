

- Core MIDI
- MIDICIResponder
-  notify(\_:onChannel:isEnabled:) Deprecated

Instance Method

# notify(\_:onChannel:isEnabled:)

Enables or disables a profile and notifies all connected initiators.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func notify(
    _ aProfile: MIDICIProfile,
    onChannel channel: MIDIChannelNumber,
    isEnabled enabledState: Bool
) -> Bool
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`aProfile`  

The profile to update.

`channel`  

The MIDI channel.

`enabledState`  

A Boolean value that indicates whether to enable the profile.

## See Also

### Broadcasting Profile Changes

func send(MIDICIProfile, onChannel: MIDIChannelNumber, profileData: Data) -> Bool

Sends profile-specific data to all connected initiators.

Deprecated

