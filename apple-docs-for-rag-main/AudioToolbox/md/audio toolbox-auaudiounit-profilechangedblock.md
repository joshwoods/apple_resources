

- Audio Toolbox
- AUAudioUnit
-  profileChangedBlock 

Instance Property

# profileChangedBlock

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
var profileChangedBlock: AUMIDICIProfileChangedBlock? { get set }
```

## See Also

### Configuring the Channel Capabilities

var channelCapabilities: [NSNumber]?

Expresses valid combinations of input and output channels.

var channelMap: [NSNumber]?

func profileState(forCable: UInt8, channel: MIDIChannelNumber) -> MIDICIProfileState

func enable(MIDICIProfile, cable: UInt8, onChannel: MIDIChannelNumber) throws

func disableProfile(MIDICIProfile, cable: UInt8, onChannel: MIDIChannelNumber) throws

