

- AVFAudio
-  AVAudioEnvironmentDistanceAttenuationParameters 

Class

# AVAudioEnvironmentDistanceAttenuationParameters

An object that specifies the amount of attenuation distance, the gradual loss in audio intensity, and other characteristics.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioEnvironmentDistanceAttenuationParameters
```

## Overview

Important

A source object (for example, AVAudioEnvironmentNode) provides an instance to this object. You can’t create standalone instances.

## Topics

### Getting and Setting the Attenuation Model

var distanceAttenuationModel: AVAudioEnvironmentDistanceAttenuationModel

The distance attenuation model that describes the drop-off in gain as the source moves away from the listener.

enum AVAudioEnvironmentDistanceAttenuationModel

Types of distance attenuation models.

### Getting and Setting the Attenuation Values

var maximumDistance: Float

The distance beyond which the node applies no further attenuation, in meters.

var referenceDistance: Float

The minimum distance at which the node applies attenuation, in meters.

var rolloffFactor: Float

A factor that determines the attenuation curve.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Spatial audio

class AVAudioEnvironmentNode

An object that simulates a 3D audio environment.

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

