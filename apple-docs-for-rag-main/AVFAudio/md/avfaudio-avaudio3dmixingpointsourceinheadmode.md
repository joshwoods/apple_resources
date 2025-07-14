

- AVFAudio
-  AVAudio3DMixingPointSourceInHeadMode 

Enumeration

# AVAudio3DMixingPointSourceInHeadMode

The in-head modes for a point source.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum AVAudio3DMixingPointSourceInHeadMode
```

## Overview

The in-head mode that determines what happens when a AVAudio3DMixingSourceMode.pointSource moves inside the head of the listener. The in-head mode applies when using the AVAudio3DMixingRenderingAlgorithm.auto rendering algorithm.

## Topics

### In-Head Modes

case mono

The point source remains a single mono source inside the head of the listener regardless of the channels it consists of.

case bypass

The point source distributes into each output channel inside the head of the listener.

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

enum AVAudioEnvironmentOutputType

The output types for using with the automatic 3D mixing rendering algorithm.

typealias AVAudio3DVector

A structure that represents a vector in 3D space, in degrees.

