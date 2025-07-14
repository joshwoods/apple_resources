

- AVFAudio
-  AVAudio3DMixing 

Protocol

# AVAudio3DMixing

A collection of properties that define 3D mixing properties.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVAudio3DMixing : NSObjectProtocol
```

## Overview

Only the AVAudioEnvironmentNode class implements these properties.

Important

The AVAudioMixing protocol adopts these properties. As a result, many classes inherit this protocol by adopting `AVAudioMixing`.

## Topics

### Getting the 3D Mixing Parameters

var obstruction: Float

A value that simulates filtering of the direct path of sound due to an obstacle.

**Required**

var occlusion: Float

A value that simulates filtering of the direct and reverb paths of sound due to an obstacle.

**Required**

var position: AVAudio3DPoint

The location of the source in the 3D environment.

**Required**

var rate: Float

A value that changes the playback rate of the input signal.

**Required**

var pointSourceInHeadMode: AVAudio3DMixingPointSourceInHeadMode

The in-head mode for a point source.

**Required**

var reverbBlend: Float

A value that controls the blend of dry and reverb processed audio.

**Required**

var sourceMode: AVAudio3DMixingSourceMode

The source mode for the input bus of the audio environment node.

**Required**

### Getting and Setting the Rendering Algorithm

var renderingAlgorithm: AVAudio3DMixingRenderingAlgorithm

The type of rendering algorithm the mixer uses.

**Required**

enum AVAudio3DMixingRenderingAlgorithm

The types of rendering algorithms available per input bus of the environment node.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- AVAudioMixing

### Conforming Types

- AVAudioEnvironmentNode
- AVAudioInputNode
- AVAudioMixerNode
- AVAudioMixingDestination
- AVAudioPlayerNode
- AVAudioSourceNode
- AVAudioUnitGenerator
- AVAudioUnitMIDIInstrument
- AVAudioUnitSampler

## See Also

### Spatial audio

class AVAudioEnvironmentNode

An object that simulates a 3D audio environment.

class AVAudioEnvironmentDistanceAttenuationParameters

An object that specifies the amount of attenuation distance, the gradual loss in audio intensity, and other characteristics.

class AVAudioEnvironmentReverbParameters

A class that encapsulates the parameters that you use to control the reverb of the environment node class.

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

enum AVAudio3DMixingPointSourceInHeadMode

The in-head modes for a point source.

typealias AVAudio3DVector

A structure that represents a vector in 3D space, in degrees.

