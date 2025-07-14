

- AVFAudio
-  AVAudioMixerNode 

Class

# AVAudioMixerNode

An object that takes any number of inputs and converts them into a single output.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioMixerNode
```

## Overview

The mixer accepts input at any sample rate and efficiently combines sample rate conversions. It also accepts any channel count and correctly upmixes or downmixes to the output channel count.

## Topics

### Creating a Mixer Node

init()

Creates an audio mixer node.

### Getting and Setting the Mixer Volume

var outputVolume: Float

The mixer’s output volume.

### Getting an Input Bus

var nextAvailableInputBus: AVAudioNodeBus

An audio bus that isn’t in a connected state.

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

### Mixing

protocol AVAudioMixing

A collection of properties that are applicable to the input bus of a mixer node.

