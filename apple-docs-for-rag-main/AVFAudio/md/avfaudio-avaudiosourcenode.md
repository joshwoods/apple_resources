

- AVFAudio
-  AVAudioSourceNode 

Class

# AVAudioSourceNode

An object that supplies audio data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class AVAudioSourceNode
```

## Overview

The `AVAudioSourceNode` class allows for supplying audio data for rendering through AVAudioSourceNodeRenderBlock. It’s a convenient method for delievering audio data instead of setting the input callback on an audio unit with `kAudioUnitProperty_SetRenderCallback`.

## Topics

### Creating an Audio Source Node

typealias AVAudioSourceNodeRenderBlock

A block that supplies audio data to an audio source node.

init(renderBlock: AVAudioSourceNodeRenderBlock)

Creates an audio source node with a block that supplies audio data.

init(format: AVAudioFormat, renderBlock: AVAudioSourceNodeRenderBlock)

Creates an audio source node with the audio format and a block that supplies audio data.

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

### Rendering

Building a signal generator

Use an audio source node and a custom render callback to generate audio signals.

Performing offline audio processing

Add offline audio processing features to your app by enabling offline manual rendering mode.

class AVAudioSinkNode

An object that receives audio data.

