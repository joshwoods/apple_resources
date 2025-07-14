

- AVFAudio
-  AVAudioEnvironmentOutputType 

Enumeration

# AVAudioEnvironmentOutputType

The output types for using with the automatic 3D mixing rendering algorithm.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum AVAudioEnvironmentOutputType
```

## Overview

The output type determines the rendering method for any input bus using AVAudio3DMixingRenderingAlgorithm.auto. To configure the output type, set outputType on AVAudioEnvironmentNode.

## Topics

### Output Types

case auto

Automatically detects the playback route and picks the correct output.

case headphones

Renders the audio output for headphones.

case builtInSpeakers

Renders the audio output for built-in speakers on the current hardware.

case externalSpeakers

Renders the audio output for external speakers according to the audio environment node’s output channel layout.

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

### Spatial audio

class AVAudioEnvironmentNode

An object that simulates a 3D audio environment.

class AVAudioEnvironmentDistanceAttenuationParameters

An object that specifies the amount of attenuation distance, the gradual loss in audio intensity, and other characteristics.

class AVAudioEnvironmentReverbParameters

A class that encapsulates the parameters that you use to control the reverb of the environment node class.

protocol AVAudio3DMixing

A collection of properties that define 3D mixing properties.

struct AVAudio3DPoint

A structure that represents a point in 3D space.

struct AVAudio3DVectorOrientation

A structure that represents two orthogonal vectors that describe the orientation of the listener in 3D space.

struct AVAudio3DAngularOrientation

A structure that represents the angular orientation of the listener in 3D space.

enum AVAudio3DMixingSourceMode

The source modes for the input bus of the audio environment node.

enum AVAudio3DMixingRenderingAlgorithm

The types of rendering algorithms available per input bus of the environment node.

enum AVAudio3DMixingPointSourceInHeadMode

The in-head modes for a point source.

typealias AVAudio3DVector

A structure that represents a vector in 3D space, in degrees.

