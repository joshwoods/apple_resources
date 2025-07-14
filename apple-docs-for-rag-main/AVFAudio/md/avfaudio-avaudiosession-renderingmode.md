

- AVFAudio
- AVAudioSession
-  renderingMode 

Instance Property

# renderingMode

The current audio session’s rendering mode.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+tvOS 17.2+

``` source
var renderingMode: AVAudioSession.RenderingMode { get }
```

## Discussion

The value of this property is AVAudioSession.RenderingMode.notApplicable in the following cases:

- The currently selected port isn’t of type carAudio or, in iOS 18 and later, airPlay.

- Your app uses a playback API other than AVPlayer or AVSampleBufferAudioRenderer.

- Playback isn’t currently active.

- The audio session is inactive, muted, or not eligible for Now Playing.

## See Also

### Inspecting rendering mode and capabilities

enum RenderingMode

Audio session rendering mode identifiers.

class let renderingModeChangeNotification: NSNotification.Name

A notification the system posts when the rendering mode changes.

var supportedOutputChannelLayouts: [AVAudioChannelLayout]

The array of channel layouts that the current route supports.

class let renderingCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when the rendering capabilities change.

