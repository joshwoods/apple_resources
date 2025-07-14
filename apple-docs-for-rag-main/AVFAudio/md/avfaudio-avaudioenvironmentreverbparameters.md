

- AVFAudio
-  AVAudioEnvironmentReverbParameters 

Class

# AVAudioEnvironmentReverbParameters

A class that encapsulates the parameters that you use to control the reverb of the environment node class.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioEnvironmentReverbParameters
```

## Overview

Use reverberation to simulate the acoustic characteristics of an environment. The AVAudioEnvironmentNode class has a built-in reverb that describe the space that the listener is in.

The reverb has a single filter that sits at the end of the chain. You use this filter to shape the overall sound of the reverb. For instance, select one of the reverb presets to simulate the general space, and then use the filter to brighten or darken the overall sound.

You can’t create a standalone instance of AVAudioEnvironmentReverbParameters. Only an instance vended by a source object is valid, such as an AVAudioEnvironmentNode instance.

## Topics

### Enabling and Disabling Reverb

var enable: Bool

A Boolean value that indicates whether reverberation is in an enabled state.

### Getting and Setting Reverb Values

var level: Float

Controls the amount of reverb, in decibels.

var filterParameters: AVAudioUnitEQFilterParameters

A filter that the system applies to the output.

func loadFactoryReverbPreset(AVAudioUnitReverbPreset)

Loads one of the reverbs factory presets.

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

class AVAudioEnvironmentDistanceAttenuationParameters

An object that specifies the amount of attenuation distance, the gradual loss in audio intensity, and other characteristics.

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

