

- RealityKit
- Entity
-  playAudio(\_:) 

Instance Method

# playAudio(\_:)

Prepares and plays a new audio playback instance on this entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@discardableResult @MainActor @preconcurrency
func playAudio(_ resource: AudioResource) -> AudioPlaybackController
```

## Parameters 

`resource`  

The audio resource the method plays. Load an audio resource from the file system with init(named:in:configuration:) , or from a URL with init(contentsOf:withName:configuration:).

## Return Value

An AudioPlaybackController object that you can use to start and stop audio playback for this specific instance of a resource playing on this entity. You can also use this controller to update playback properties, such as gain and speed, during playback.

## Discussion

The method prepares the audio by calling prepareAudio(_:), and then immediately calls the play() method of the controller that it returns. To begin multiple playback instances you can call `playAudio` multiple times.

## See Also

### Playing audio

func playAudio(configuration: AudioGeneratorConfiguration, Audio.GeneratorRenderHandler) throws -> AudioGeneratorController

Prepares and plays a real-time audio playback instance.

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

