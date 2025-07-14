

- AVFAudio
- AVAudioSession
-  renderingCapabilitiesChangeNotification 

Type Property

# renderingCapabilitiesChangeNotification

A notification the system posts when the rendering capabilities change.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+tvOS 17.2+

``` source
class let renderingCapabilitiesChangeNotification: NSNotification.Name
```

## See Also

### Inspecting rendering mode and capabilities

var renderingMode: AVAudioSession.RenderingMode

The current audio session’s rendering mode.

enum RenderingMode

Audio session rendering mode identifiers.

class let renderingModeChangeNotification: NSNotification.Name

A notification the system posts when the rendering mode changes.

var supportedOutputChannelLayouts: [AVAudioChannelLayout]

The array of channel layouts that the current route supports.

