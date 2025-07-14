

- AVFAudio
- AVAudioSession
-  supportedOutputChannelLayouts 

Instance Property

# supportedOutputChannelLayouts

The array of channel layouts that the current route supports.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+tvOS 17.2+

``` source
var supportedOutputChannelLayouts: [AVAudioChannelLayout] { get }
```

## Discussion

The possible channel layouts for this property are:

- kAudioChannelLayoutTag_Stereo

- kAudioChannelLayoutTag_AAC_5_1

- kAudioChannelLayoutTag_MPEG_7_1_C

- kAudioChannelLayoutTag_Atmos_5_1_2

- kAudioChannelLayoutTag_Atmos_5_1_4

- kAudioChannelLayoutTag_Atmos_7_1_2

- kAudioChannelLayoutTag_Atmos_7_1_4

- kAudioChannelLayoutTag_Atmos_9_1_6

This value returns an empty array when the audio session is inactive, ineligible for Now Playing, or the port type isn’t carAudio or, in iOS 18 or later, airPlay.

Use renderingCapabilitiesChangeNotification to listen for updates from the system.

## See Also

### Inspecting rendering mode and capabilities

var renderingMode: AVAudioSession.RenderingMode

The current audio session’s rendering mode.

enum RenderingMode

Audio session rendering mode identifiers.

class let renderingModeChangeNotification: NSNotification.Name

A notification the system posts when the rendering mode changes.

class let renderingCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when the rendering capabilities change.

