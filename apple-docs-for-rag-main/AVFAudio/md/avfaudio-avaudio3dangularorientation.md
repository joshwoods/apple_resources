

- AVFAudio
-  AVAudio3DAngularOrientation 

Structure

# AVAudio3DAngularOrientation

A structure that represents the angular orientation of the listener in 3D space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVAudio3DAngularOrientation
```

## Overview

This represents the three angles that describe the orientation of a listener’s head — yaw, pitch, and roll.

## Topics

### Creating an Angular Orientation

init()

Creates an angular orientation.

init(yaw: Float, pitch: Float, roll: Float)

Creates a 3D angular orientation using the yaw, pitch, and roll values you specify.

func AVAudioMake3DAngularOrientation(Float, Float, Float) -> AVAudio3DAngularOrientation

Creates a 3D angular orientation using the yaw, pitch, and roll values you specify.

### Getting Angular Orientation Properties

var yaw: Float

The side-to-side movement of the listener’s head.

var pitch: Float

The up-and-down movement of the listener’s head.

var roll: Float

The tilt of the listener’s head.

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

struct AVAudio3DVectorOrientation

A structure that represents two orthogonal vectors that describe the orientation of the listener in 3D space.

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

