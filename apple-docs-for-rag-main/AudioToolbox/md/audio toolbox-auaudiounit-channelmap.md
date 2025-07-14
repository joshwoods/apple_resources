

- Audio Toolbox
- AUAudioUnit
-  channelMap 

Instance Property

# channelMap

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var channelMap: [NSNumber]? { get set }
```

## See Also

### Configuring the Channel Capabilities

var channelCapabilities: [NSNumber]?

Expresses valid combinations of input and output channels.

func profileState(forCable: UInt8, channel: MIDIChannelNumber) -> MIDICIProfileState

func enable(MIDICIProfile, cable: UInt8, onChannel: MIDIChannelNumber) throws

func disableProfile(MIDICIProfile, cable: UInt8, onChannel: MIDIChannelNumber) throws

var profileChangedBlock: AUMIDICIProfileChangedBlock?

