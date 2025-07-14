

- AVFAudio
-  AVAudioEnvironmentNode 

Class

# AVAudioEnvironmentNode

An object that simulates a 3D audio environment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioEnvironmentNode
```

## Overview

The `AVAudioEnvironmentNode` class is a mixer node that simulates a 3D audio environment. Any node that conforms to AVAudioMixing can act as a source node, such as AVAudioPlayerNode.

The environment node has an implicit listener. You set the listener’s position and orientation, and the system then controls the way the user experiences the virtual world.

To help characterize the environment, this class defines properties for distance attenuation and reverberation.

AVAudio3DMixingSourceMode affects how inputs with different channel configurations render. Spatialization applies only to inputs with a mono channel connection format. This class doesn’t spatialize stereo inputs or support inputs with connection formats of more than two channels.

To set the node’s output to a multichannel format, use an AVAudioFormat that has one of the following Audio Channel Layout Tags:

- kAudioChannelLayoutTag_AudioUnit_4

- kAudioChannelLayoutTag_AudioUnit_5_0

- kAudioChannelLayoutTag_AudioUnit_6_0

- kAudioChannelLayoutTag_AudioUnit_7_0

- kAudioChannelLayoutTag_AudioUnit_7_0_Front

- kAudioChannelLayoutTag_AudioUnit_8

## Topics

### Creating an Environment Node

init()

Creates a new environment node object.

### Getting and Setting Positional Properties

var listenerPosition: AVAudio3DPoint

The listener’s position in the 3D environment.

var listenerAngularOrientation: AVAudio3DAngularOrientation

The listener’s angular orientation in the environment.

var listenerVectorOrientation: AVAudio3DVectorOrientation

The listener’s vector orientation in the environment.

### Getting Attenuation and Reverb Properties

var distanceAttenuationParameters: AVAudioEnvironmentDistanceAttenuationParameters

The distance attenuation parameters for the environment.

var reverbParameters: AVAudioEnvironmentReverbParameters

The reverb parameters for the environment.

### Getting and Setting Environment Properties

var outputVolume: Float

The mixer’s output volume.

var outputType: AVAudioEnvironmentOutputType

The type of output hardware.

### Getting the Available Rendering Algorithms

var applicableRenderingAlgorithms: [NSNumber]

An array of rendering algorithms applicable to the environment node.

### Getting the Head Tracking Status

var isListenerHeadTrackingEnabled: Bool

A Boolean value that indicates whether the listener orientation is automatically rotated based on head orientation.

### Getting the Input Bus

var nextAvailableInputBus: AVAudioNodeBus

An unused input bus.

## Relationships

### Inherits From

- AVAudioNode

### Conforms To

- AVAudio3DMixing
- AVAudioMixing
- AVAudioStereoMixing
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Spatial audio

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

enum AVAudio3DMixingPointSourceInHeadMode

The in-head modes for a point source.

typealias AVAudio3DVector

A structure that represents a vector in 3D space, in degrees.

