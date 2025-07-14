

- AVFAudio
-  AVAudio3DMixingRenderingAlgorithm 

Enumeration

# AVAudio3DMixingRenderingAlgorithm

The types of rendering algorithms available per input bus of the environment node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum AVAudio3DMixingRenderingAlgorithm
```

## Overview

The rendering algorithms differ in quality and CPU cost. AVAudio3DMixingRenderingAlgorithm.equalPowerPanning is the simplest panning algorithm and the least expensive computationally.

When rendering to multichannel hardware, most of the rendering algorithms only render to channels 1 and 2, excluding AVAudio3DMixingRenderingAlgorithm.soundField and AVAudio3DMixingRenderingAlgorithm.auto.

## Topics

### Rendering Algorithms

case auto

Automatically selects the highest-quality rendering algorithm available for the current playback hardware.

case equalPowerPanning

An algorithm that pans the data of the mixer bus into a stereo field.

case HRTF

A high-quality algorithm that uses filtering to emulate 3D space in headphones.

case HRTFHQ

A higher-quality head-related transfer function rendering algorithm.

case soundField

An algorithm that renders to multichannel hardware.

case sphericalHead

An algorithm that emulates 3D space in headphones by simulating interaural time delays and other spatial cues.

case stereoPassThrough

An algorithm to use when the source data doesn’t need localization.

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

enum AVAudioEnvironmentOutputType

The output types for using with the automatic 3D mixing rendering algorithm.

enum AVAudio3DMixingPointSourceInHeadMode

The in-head modes for a point source.

typealias AVAudio3DVector

A structure that represents a vector in 3D space, in degrees.

