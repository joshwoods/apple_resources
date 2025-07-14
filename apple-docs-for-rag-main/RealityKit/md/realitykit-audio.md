

- RealityKit
-  Audio 

API Collection

# Audio

Create personalized and realistic spatial audio experiences.

## Overview

Creating a compelling audio experience with RealityKit is as simple as playing audio on your existing RealityKit entities. Use RealityKit’s default audio settings to create a personalized and realistic experience or utilize advanced customization options to tailor the audio for the needs of your application. Utilizing acoustic ray tracing and a personalized HRTF, RealityKit provides lifelike and high-quality sound.

You can load and configure audio with an AudioResource subclass, such as AudioFileResource, and adjust the spatial rendering with SpatialAudioComponent, AmbientAudioComponent, ChannelAudioComponent. Control the audio resource playback with AudioPlaybackController. For real-time audio playback you can prepare a Audio.GeneratorRenderHandler and control playback with AudioGeneratorController. You can control the playback levels of multiple resources at once with AudioMixGroup and AudioMixGroupsComponent.

## Topics

### Audio source components

Creating a Spaceship game

Build an immersive game using RealityKit audio, simulation, and rendering features.

struct SpatialAudioComponent

A component that configures how sounds emit from an entity into a person’s environment.

struct AmbientAudioComponent

A component that configures the ambient rendering of sounds from an entity.

struct ChannelAudioComponent

A component that configures channel-based rendering of sounds from an entity.

### Playback controllers

class AudioPlaybackController

A controller that manages an audio playback instance.

class AudioGeneratorController

A controller that manages the playback of a real-time audio stream.

struct AudioGeneratorConfiguration

A container for various settings for preparing and playing an AudioGeneratorController.

enum AudioEvents

Events associated with audio playback.

struct PlayAudioAction

An action which plays an audio resource on the given target entity.

### Audio resources

class AudioFileResource

An audio resource that you load from a file or from a URL.

class AudioFileGroupResource

An audio file group.

class AudioBufferResource

An audio resource that you load from an AVAudioBuffer.

struct AudioLibraryComponent

A container for audio resources that you can look up by user-defined names.

class AudioResource

A playable audio resource

struct Calibration

A container for different calibration modes that can be applied for playback.

struct Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.

### Reverb

struct Reverb

The reverberation RealityKit applies to spatial audio sources.

struct Preset

Reverbs defined by a preset environment.

struct ReverbComponent

A component that defines the reverberation of spatial audio sources.

### Audio mixing

struct AudioMixGroup

A group that manages the playback properties of multiple playing sounds.

struct AudioMixGroupsComponent

A component that provides functionality for controlling the playback of audio you assign to mix groups in a scene.

### Audio types

enum Audio

A namespace for types that are used commonly in audio.

typealias Decibel

The unit for measuring intensity of sound on a logarithmic scale.

enum Directivity

The radiation pattern of sound emitted from an entity.

enum DistanceAttenuation

The different ways that audio intensity diminishes as the distance between the listener and the sound source increases.

## See Also

### Scene content

Hello World

Use windows, volumes, and immersive spaces to teach people about the Earth.

Enabling video reflections in an immersive environment

Create a more immersive experience by adding video reflections in a custom environment.

Creating a spatial drawing app with RealityKit

Use low-level mesh and texture APIs to achieve fast updates to a person’s brush strokes by integrating RealityKit with ARKit and SwiftUI.

Generating interactive geometry with RealityKit

Create an interactive mesh with low-level mesh and low-level texture.

Combining 2D and 3D views in an immersive app

Use attachments to place 2D content relative to 3D content in your visionOS app.

Transforming RealityKit entities using gestures

Build a RealityKit component to support standard visionOS gestures on any entity.

Models and meshes

Display virtual objects in your scene with mesh-based models.

Materials, textures, and shaders

Apply textures to the surface of your scene’s 3D objects to give each object a unique appearance.

Anchors

Lock virtual content to the real world.

Lights and cameras

Control the lighting and point of view for a scene.

Content synchronization

Synchronize the contents of entities locally or across the network.

Videos

Present videos in your RealityKit experiences.

