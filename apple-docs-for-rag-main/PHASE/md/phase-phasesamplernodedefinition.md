

- PHASE
-  PHASESamplerNodeDefinition 

Class

# PHASESamplerNodeDefinition

A node that plays complete audio data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESamplerNodeDefinition
```

## Overview

Generate sound events from this node to play audio data that your app loads completely, either from disk or from memory.

## Topics

### Creating a Sampler Node

init(soundAssetIdentifier: String, mixerDefinition: PHASEMixerDefinition)

Creates a sampler node with the given sound asset and mixer.

convenience init(soundAssetIdentifier: String, mixerDefinition: PHASEMixerDefinition, identifier: String)

Creates a named sampler node with the given sound asset and mixer.

### Identifying the Audio

var assetIdentifier: String

The name of the audio this node plays.

### Defining Cull Behavior

var cullOption: PHASECullOption

The action the engine performs after it temporarily removes the node’s sound from the audio output.

enum PHASECullOption

The actions the engine takes when it culls sound.

### Looping the Audio

var playbackMode: PHASEPlaybackMode

An option that determines whether the node’s audio plays in a loop.

## Relationships

### Inherits From

- PHASEGeneratorNodeDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio-Providing Nodes

enum PHASEPlaybackMode

Loop options for audio playback.

class PHASEPushStreamNodeDefinition

A node that plays a sequence of audio buffers.

class PHASEPushStreamNode

An audio stream you manage to provide a sound buffer data.

struct PHASEPushStreamBufferOptions

Options that inform PHASE of an audio-stream buffer’s playback priority.

enum PHASECalibrationMode

Calibration options for sound pressure level.

class PHASEGeneratorNodeDefinition

A base class for nodes that provide audio data to generate sound.

