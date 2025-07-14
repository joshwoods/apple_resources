

- RealityKit
- Entity
-  prepareAudio(\_:) 

Instance Method

# prepareAudio(\_:)

Prepares an audio resource for playback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func prepareAudio(_ resource: AudioResource) -> AudioPlaybackController
```

## Parameters 

`resource`  

The audio resource the method plays. Load an audio resource from the file system with init(named:in:configuration:) , or from a URL with init(contentsOf:withName:configuration:).

## Return Value

An AudioPlaybackController object that you can use to start and stop audio playback for this specific instance of a resource playing on this entity. You can also use this controller to update playback properties, such as gain and speed, during playback.

## Discussion

To start playback right away with default `AudioPlaybackController` properties, use the playAudio(_:) method instead.

Note

As soon as the system prepares an audio resource, the audio engine begins tracking the position of the entity and allocates rendering resources, which incurs a power cost.

For optimal system resource usage, avoid preparing sounds before they are needed. For example:

```
let controller = entity.prepareAudio(anAudioResource)
controller.gain = -10 // Apply a custom gain, if desired.
controller.speed = 1.2 // Apply a custom speed, if desired.
controller.play()
```

## See Also

### Playing audio

func playAudio(AudioResource) -> AudioPlaybackController

Prepares and plays a new audio playback instance on this entity.

func playAudio(configuration: AudioGeneratorConfiguration, Audio.GeneratorRenderHandler) throws -> AudioGeneratorController

Prepares and plays a real-time audio playback instance.

func prepareAudio(configuration: AudioGeneratorConfiguration, Audio.GeneratorRenderHandler) throws -> AudioGeneratorController

Prepares a real-time audio playback instances.

func stopAllAudio()

Stops playback for all audio on this entity.

var spatialAudio: SpatialAudioComponent?

The component that configures the spatial rendering of sounds from this entity.

var ambientAudio: AmbientAudioComponent?

The component that configures the ambient rendering of sounds from this entity.

var channelAudio: ChannelAudioComponent?

The component that configures the channel-based rendering of sounds from this entity.

