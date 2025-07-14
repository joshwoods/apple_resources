

- AVFAudio
-  AVAudio3DVectorOrientation 

Structure

# AVAudio3DVectorOrientation

A structure that represents two orthogonal vectors that describe the orientation of the listener in 3D space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVAudio3DVectorOrientation
```

## Overview

Two orthogonal vectors describe the orientation of the listener. The forward vector points in the direction the listener faces. The up vector is orthogonal to the forward vector and points upward from the listener’s head.

## Topics

### Creating a Vector Orientation

init()

Creates a 3D vector orientation instance.

init(forward: AVAudio3DVector, up: AVAudio3DVector)

Creates a 3D vector orientation instance using the forward and up vectors you specify.

func AVAudioMake3DVectorOrientation(AVAudio3DVector, AVAudio3DVector) -> AVAudio3DVectorOrientation

Creates a 3D vector orientation instance using the forward and up vectors you specify.

### Getting Vector Orientation Properties

var forward: AVAudio3DVector

The forward vector points in the direction that the listener faces.

var up: AVAudio3DVector

The up vector is orthogonal to the forward vector and points upward from the listener’s head.

## Relationships

### Conforms To

- BitwiseCopyable
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

struct AVAudio3DAngularOrientation

A structure that represents the angular orientation of the listener in 3D space.

enum AVAudio3DMixingSourceMode

The source modes for the input bus of the audio environment node.

enum AVAudio3DMixingRenderingAlgorithm

The types of rendering algorithms available per input bus of the environment node.

enum AVAudioEnvironmentOutputType

The output types for using with the automatic 3D mixing rendering algorithm.

enum AVAudio3DMixingPointSourceInHeadMode

The in-head modes for a point source.

typealias AVAudio3DVector

A structure that represents a vector in 3D space, in degrees.

