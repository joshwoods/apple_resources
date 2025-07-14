

- RealityKit
-  AudioGeneratorController 

Class

# AudioGeneratorController

A controller that manages the playback of a real-time audio stream.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
class AudioGeneratorController
```

## Overview

To receive an audio generator controller, call an entity’s prepareAudio(configuration:_:) or playAudio(configuration:_:) method.

The following examples show how you can use the controller:

```
```

```
// Create a configuration.
var config = AudioGeneratorConfiguration(kAudioChannelLayoutTag_Mono)

// Prepare a closure that you define in myHandler.mm.
var controller = myEntity.prepareAudio(configuration: config, myHandler)

controller.gain = -3.0
controller.play()
```

During playback, the audio appears to come from the entity that you use to create the controller. As a person moves around the MR scene, RealityKit modulates the characteristics of the audio to account for their location.

Note

Audio stops rendering when the system deallocates `AudioGeneratorController`. Create another `AudioGeneratorController` to restart audio.

Call stop() to halt the audio, and play() to restart the stream.

## Topics

### Instance Properties

let configuration: AudioGeneratorConfiguration

The configuration with rendering parameters for the render handler.

var entity: Entity?

The entity the audio stream emanates from.

var gain: Audio.Decibel

The gain in decibels of the audio generator controller output.

var isPlaying: Bool

A Boolean value that indicates whether playback is currently active.

### Instance Methods

func play()

Begins the audio stream from the generator render handler.

func stop()

Stops playback of the render handler.

## Relationships

### Conforms To

- Sendable

## See Also

### Playback controllers

class AudioPlaybackController

A controller that manages an audio playback instance.

struct AudioGeneratorConfiguration

A container for various settings for preparing and playing an AudioGeneratorController.

enum AudioEvents

Events associated with audio playback.

struct PlayAudioAction

An action which plays an audio resource on the given target entity.

