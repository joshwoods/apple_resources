

- RealityKit
- Entity
-  playAudio(configuration:\_:) 

Instance Method

# playAudio(configuration:\_:)

Prepares and plays a real-time audio playback instance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
func playAudio(
    configuration: AudioGeneratorConfiguration = .init(),
    _ generatorRenderHandler: @escaping Audio.GeneratorRenderHandler
) throws -> AudioGeneratorController
```

## Parameters 

`configuration`  

A set of configuration parameters necessary for initializing and rendering the `generatorRenderHandler`.

`generatorRenderHandler`  

The audio render handler to play. The system runs this handler to generate real-time audio.

## Return Value

An AudioGeneratorController instance that you use to manage audio playback. Use the controller to set the volume and start or stop playback.

## Discussion

Maintain playback by keeping a reference to the generator controller.

## See Also

### Playing audio

func playAudio(AudioResource) -> AudioPlaybackController

Prepares and plays a new audio playback instance on this entity.

func prepareAudio(configuration: AudioGeneratorConfiguration, Audio.GeneratorRenderHandler) throws -> AudioGeneratorController

Prepares a real-time audio playback instances.

func prepareAudio(AudioResource) -> AudioPlaybackController

Prepares an audio resource for playback.

func stopAllAudio()

Stops playback for all audio on this entity.

var spatialAudio: SpatialAudioComponent?

The component that configures the spatial rendering of sounds from this entity.

var ambientAudio: AmbientAudioComponent?

The component that configures the ambient rendering of sounds from this entity.

var channelAudio: ChannelAudioComponent?

The component that configures the channel-based rendering of sounds from this entity.

