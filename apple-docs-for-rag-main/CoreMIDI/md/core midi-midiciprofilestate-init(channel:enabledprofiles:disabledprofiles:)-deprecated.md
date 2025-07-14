

- Core MIDI
- MIDICIProfileState
-  init(channel:enabledProfiles:disabledProfiles:) Deprecated

Initializer

# init(channel:enabledProfiles:disabledProfiles:)

Creates a new profile state object for the specified MIDI channel and profiles.

iOS 12.0–18.0DeprecatediPadOS 12.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
init(
    channel midiChannelNum: MIDIChannelNumber,
    enabledProfiles enabled: [MIDICIProfile],
    disabledProfiles disabled: [MIDICIProfile]
)
```

## Parameters 

`midiChannelNum`  

The MIDI channel.

`enabled`  

The enabled MIDI-CI profles.

`disabled`  

The disabled MIDI-CI profles.

## See Also

### Creating a Profile State

init(enabledProfiles: [MIDICIProfile], disabledProfiles: [MIDICIProfile])

Creates a new profile state object for the specified profiles.

Deprecated

