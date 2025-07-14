

- RealityKit
- Entity
-  spatialAudio 

Instance Property

# spatialAudio

The component that configures the spatial rendering of sounds from this entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
var spatialAudio: SpatialAudioComponent? { get set }
```

## See Also

### Playing audio

func playAudio(AudioResource) -> AudioPlaybackController

Prepares and plays a new audio playback instance on this entity.

func playAudio(configuration: AudioGeneratorConfiguration, Audio.GeneratorRenderHandler) throws -> AudioGeneratorController

Prepares and plays a real-time audio playback instance.

func prepareAudio(configuration: AudioGeneratorConfiguration, Audio.GeneratorRenderHandler) throws -> AudioGeneratorController

Prepares a real-time audio playback instances.

func prepareAudio(AudioResource) -> AudioPlaybackController

Prepares an audio resource for playback.

func stopAllAudio()

Stops playback for all audio on this entity.

var ambientAudio: AmbientAudioComponent?

The component that configures the ambient rendering of sounds from this entity.

var channelAudio: ChannelAudioComponent?

The component that configures the channel-based rendering of sounds from this entity.

