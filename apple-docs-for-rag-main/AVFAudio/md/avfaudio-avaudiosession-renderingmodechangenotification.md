

- AVFAudio
- AVAudioSession
-  renderingModeChangeNotification 

Type Property

# renderingModeChangeNotification

A notification the system posts when the rendering mode changes.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+tvOS 17.2+

``` source
class let renderingModeChangeNotification: NSNotification.Name
```

## Topics

### User information keys

let AVAudioSessionRenderingModeNewRenderingModeKey: String

A key to retrieve an integer value that represents the new resolved rendering mode.

## See Also

### Inspecting rendering mode and capabilities

var renderingMode: AVAudioSession.RenderingMode

The current audio session’s rendering mode.

enum RenderingMode

Audio session rendering mode identifiers.

var supportedOutputChannelLayouts: [AVAudioChannelLayout]

The array of channel layouts that the current route supports.

class let renderingCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when the rendering capabilities change.

