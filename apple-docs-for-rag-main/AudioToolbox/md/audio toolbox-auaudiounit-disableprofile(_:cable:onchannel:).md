

- Audio Toolbox
- AUAudioUnit
-  disableProfile(\_:cable:onChannel:) 

Instance Method

# disableProfile(\_:cable:onChannel:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
func disableProfile(
    _ profile: MIDICIProfile,
    cable: UInt8,
    onChannel channel: MIDIChannelNumber
) throws
```

## See Also

### Configuring the Channel Capabilities

var channelCapabilities: [NSNumber]?

Expresses valid combinations of input and output channels.

var channelMap: [NSNumber]?

func profileState(forCable: UInt8, channel: MIDIChannelNumber) -> MIDICIProfileState

func enable(MIDICIProfile, cable: UInt8, onChannel: MIDIChannelNumber) throws

var profileChangedBlock: AUMIDICIProfileChangedBlock?

