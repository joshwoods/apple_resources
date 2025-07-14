

- AVFAudio
-  AVAudio3DPoint 

Structure

# AVAudio3DPoint

A structure that represents a point in 3D space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVAudio3DPoint
```

## Overview

Classes that deal with 3D audio, such as those adopting AVAudioMixing and AVAudioEnvironmentNode, use this structure. The system represents this point in meters.

## Topics

### Creating a Point

init()

Creates a 3D point.

init(x: Float, y: Float, z: Float)

Creates a 3D point using the x, y, and z coordinates you specify.

func AVAudioMake3DPoint(Float, Float, Float) -> AVAudio3DPoint

Creates a 3D point using the x, y, and z coordinates you specify.

### Getting Point Properties

var x: Float

The location on the x-axis, in meters.

var y: Float

The location on the y-axis, in meters.

var z: Float

The location on the z-axis, in meters.

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

enum AVAudio3DMixingPointSourceInHeadMode

The in-head modes for a point source.

typealias AVAudio3DVector

A structure that represents a vector in 3D space, in degrees.

