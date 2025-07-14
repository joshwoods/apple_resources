

- AVFAudio
-  AVAudio3DVector 

Type Alias

# AVAudio3DVector

A structure that represents a vector in 3D space, in degrees.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVAudio3DVector = AVAudio3DPoint
```

## Discussion

Classes that deal with 3D audio use this structure, such as those that adopt the AVAudioMixing protocol and the AVAudioEnvironmentNode class.

## Topics

### Functions

func AVAudioMake3DVector(Float, Float, Float) -> AVAudio3DVector

Creates a vector in 3D space, in degrees.

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

enum AVAudio3DMixingPointSourceInHeadMode

The in-head modes for a point source.

