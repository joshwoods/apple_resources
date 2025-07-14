

- AVFAudio
-  AVAudioStereoMixing 

Protocol

# AVAudioStereoMixing

A protocol that defines stereo mixing properties a mixer uses.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol AVAudioStereoMixing : NSObjectProtocol
```

## Overview

Important

The AVAudioMixing protocol adopts this protocol. As a result, many classes also inherit this protocol by adopting `AVAudioMixing`.

## Topics

### Getting and Setting the Stereo Panning

var pan: Float

The bus’s stereo pan.

**Required**

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

### Defining Mixing Properties

protocol AVAudio3DMixing

A collection of properties that define 3D mixing properties.

