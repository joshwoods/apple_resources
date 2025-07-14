

- RealityKit
-  AudioPlaybackController 

Class

# AudioPlaybackController

A controller that manages an audio playback instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class AudioPlaybackController
```

## Overview

You can obtain an audio playback controller by calling an entity’s Entity/prepareAudio(*:) or Entity/playAudio(*:) method which creates a controller with the associated AudioResource. To play multiple instances of a resource, call playAudio(_:) to obtain new AudioPlaybackControllers.

During playback, the audio appears to come from the entity that you used to create the controller. As you move around the MR scene, RealityKit modulates the characteristics of the audio to account for your location.

Note

Playback commences only after the entity is parented and placed within a scene.

After playback completes, or if you call the stop() method, the audio resource resets, allowing you to replay the resource from the beginning. Alternatively, you can enable indefinite looping by setting the `loops` property of the audio resource to `true`.

Look for one of the events in AudioEvents if you want to be alerted when certain aspects of audio playback occur.

## Topics

### Identifying the controller

var id: UInt64

The stable identity of the controller.

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Managing the resource

let resource: AudioResource

The resource that provides the audio stream.

### Setting the volume

var gain: AudioPlaybackController.Decibel

The individual gain in decibels of the audio playback controller output.

func fade(to: AudioPlaybackController.Decibel, duration: TimeInterval)

Transitions the gain to the given value over a time interval using a linear curve.

### Setting the speed

var speed: Double

The rate of playback of the audio resource, with a range of `[.25, 4]`

### Setting the reverb

var reverbSendLevel: AudioPlaybackController.Decibel

The send level from this playback controller to the reverb system.

Deprecated

### Starting and stopping audio playback

func play()

Plays the audio resource.

func pause()

Pauses playback of the audio resource while maintaining the position in the audio stream.

func stop()

Stops playback of the audio resource and discards the location in the audio stream.

var isPlaying: Bool

A Boolean value that indicates whether playback is currently active.

### Handling completion

var completionHandler: (() -> Void)?

A closure that the playback controller executes when it reaches the end of the audio stream.

### Finding the associated entity

var entity: Entity?

The entity from which the audio stream emanates.

### Instance Methods

func seek(to: Duration)

Sets the playback position to the specified time.

### Type Aliases

typealias Decibel

A type alias for Double expressing that the value is in Decibels.

### Default Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- Identifiable
- Sendable

## See Also

### Playback controllers

class AudioGeneratorController

A controller that manages the playback of a real-time audio stream.

struct AudioGeneratorConfiguration

A container for various settings for preparing and playing an AudioGeneratorController.

enum AudioEvents

Events associated with audio playback.

struct PlayAudioAction

An action which plays an audio resource on the given target entity.

