

- Core MIDI
- MIDICIProfileState
-  init(enabledProfiles:disabledProfiles:) Deprecated

Initializer

# init(enabledProfiles:disabledProfiles:)

Creates a new profile state object for the specified profiles.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    enabledProfiles enabled: [MIDICIProfile],
    disabledProfiles disabled: [MIDICIProfile]
)
```

Deprecated

Use init(channel:enabledProfiles:disabledProfiles:) instead.

## Parameters 

`enabled`  

The enabled MIDI-CI profiles.

`disabled`  

The disabled MIDI-CI profiles.

## Return Value

A new profile state instance.

## See Also

### Creating a Profile State

init(channel: MIDIChannelNumber, enabledProfiles: [MIDICIProfile], disabledProfiles: [MIDICIProfile])

Creates a new profile state object for the specified MIDI channel and profiles.

Deprecated

