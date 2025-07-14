

- PHASE
-  PHASEPushStreamNodeDefinition 

Class

# PHASEPushStreamNodeDefinition

A node that plays a sequence of audio buffers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEPushStreamNodeDefinition
```

## Overview

Use this node to create sound events for a piecemeal audio source, for example, an audio stream that your app accesses over the network or loads from a memory-mapped file on disk.

Note

To create a sound event for fully-loaded audio data instead, use PHASESamplerNodeDefinition.

## Topics

### Creating a Node

init(mixerDefinition: PHASEMixerDefinition, format: AVAudioFormat)

Creates a node definition for audio streams.

convenience init(mixerDefinition: PHASEMixerDefinition, format: AVAudioFormat, identifier: String)

Creates a named node definition for audio streams.

### Observing the Format

var format: AVAudioFormat

The format of the audio stream data.

### Shaping Loudness

var normalize: Bool

An option that resizes loudness of the audio stream for consistency.

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

class PHASESamplerNodeDefinition

A node that plays complete audio data.

enum PHASEPlaybackMode

Loop options for audio playback.

class PHASEPushStreamNode

An audio stream you manage to provide a sound buffer data.

struct PHASEPushStreamBufferOptions

Options that inform PHASE of an audio-stream buffer’s playback priority.

enum PHASECalibrationMode

Calibration options for sound pressure level.

class PHASEGeneratorNodeDefinition

A base class for nodes that provide audio data to generate sound.

