

- PHASE
-  PHASEGeneratorNodeDefinition 

Class

# PHASEGeneratorNodeDefinition

A base class for nodes that provide audio data to generate sound.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEGeneratorNodeDefinition
```

## Overview

This class encapsulates shared logic for subclasses that provide audio data to a mixer for sound output, namely PHASESamplerNodeDefinition and PHASEPushStreamNodeDefinition.

## Topics

### Calibrating Loudness

func setCalibrationMode(calibrationMode: PHASECalibrationMode, level: Double)

Selects a loudness correction strategy and reference level.

var calibrationMode: PHASECalibrationMode

A sound pressure level strategy for loudness correction.

var level: Double

The node’s loudness.

### Defining an Output Strategy

var mixerDefinition: PHASEMixerDefinition

An object that combines audio layers for the node’s output.

### Joining a Group

var group: PHASEGroup?

A group this node conforms to for gain and rate control.

### Controlling Audio Playback

var rate: Double

A playback speed for the node’s audio.

var rateMetaParameterDefinition: PHASENumberMetaParameterDefinition?

A meta parameter that dynamically changes the audio’s rate.

var gainMetaParameterDefinition: PHASENumberMetaParameterDefinition?

A meta parameter that dynamically changes the audio’s loudness.

## Relationships

### Inherits From

- PHASESoundEventNodeDefinition

### Inherited By

- PHASEPullStreamNodeDefinition
- PHASEPushStreamNodeDefinition
- PHASESamplerNodeDefinition

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

class PHASEPushStreamNodeDefinition

A node that plays a sequence of audio buffers.

class PHASEPushStreamNode

An audio stream you manage to provide a sound buffer data.

struct PHASEPushStreamBufferOptions

Options that inform PHASE of an audio-stream buffer’s playback priority.

enum PHASECalibrationMode

Calibration options for sound pressure level.

