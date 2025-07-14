

- RealityKit
-  AudioGeneratorConfiguration 

Structure

# AudioGeneratorConfiguration

A container for various settings for preparing and playing an AudioGeneratorController.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct AudioGeneratorConfiguration
```

## Topics

### Initializers

init(layoutTag: AudioChannelLayoutTag, mixGroupName: String?)

### Instance Properties

var layoutTag: AudioChannelLayoutTag

The format in which the audio channels are specified.

var mixGroupName: String?

An arbitrary name that assigns an audio resource to an audio mix group.

## See Also

### Playback controllers

class AudioPlaybackController

A controller that manages an audio playback instance.

class AudioGeneratorController

A controller that manages the playback of a real-time audio stream.

enum AudioEvents

Events associated with audio playback.

struct PlayAudioAction

An action which plays an audio resource on the given target entity.

