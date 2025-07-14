

- AVFAudio
- AVAudioSession
-  AVAudioSession.RenderingMode 

Enumeration

# AVAudioSession.RenderingMode

Audio session rendering mode identifiers.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
enum RenderingMode
```

## Topics

### Getting the rendering modes

case monoStereo

A mode that represents non multi-channel audio.

case surround

A mode that represents general multi-channel audio.

case spatialAudio

A mode that represents a fallback for when hardware capabilities don’t support Dolby.

case dolbyAudio

A mode that represents Dolby audio.

case dolbyAtmos

A mode that represents Dolby Atmos.

case notApplicable

A mode that represents there’s no asset in a loading or playing state.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting rendering mode and capabilities

var renderingMode: AVAudioSession.RenderingMode

The current audio session’s rendering mode.

class let renderingModeChangeNotification: NSNotification.Name

A notification the system posts when the rendering mode changes.

var supportedOutputChannelLayouts: [AVAudioChannelLayout]

The array of channel layouts that the current route supports.

class let renderingCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when the rendering capabilities change.

