

- PHASE
-  PHASEPlaybackMode 

Enumeration

# PHASEPlaybackMode

Loop options for audio playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASEPlaybackMode
```

## Overview

This class defines the options for a sampler node’s playbackMode. These options control whether the node’s sound event automatically plays back its audio asset from the beginning after finishing.

## Topics

### Playback Modes

case oneShot

An option that plays a sound only once.

case looping

An option that restarts a sound from the begining after it finishes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Audio-Providing Nodes

class PHASESamplerNodeDefinition

A node that plays complete audio data.

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

