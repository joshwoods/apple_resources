

- AVFAudio
-  AVAudioNode 

Class

# AVAudioNode

An object you use for audio generation, processing, or an I/O block.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioNode
```

## Overview

An AVAudioEngine object contains instances of audio nodes that you attach, and this base class provides common functionality. Instances of this class don’t provide useful functionality until you attach them to an engine.

Nodes have input and output busses that serve as connection points. For example, an effect has one input bus and one output bus, and a mixer has multiple input busses and one output bus.

A bus contains a format the framework expresses in terms of sample rate and channel count. Formats must match exactly when making connections between nodes, excluding AVAudioMixerNode and AVAudioOutputNode.

## Topics

### Configuring an Input Format Bus

typealias AVAudioNodeBus

The index of a bus on an audio node.

func inputFormat(forBus: AVAudioNodeBus) -> AVAudioFormat

Gets the input format for the bus you specify.

func name(forInputBus: AVAudioNodeBus) -> String?

Gets the name of the input bus you specify.

var numberOfInputs: Int

The number of input busses for the node.

### Creating an Output Format Bus

func outputFormat(forBus: AVAudioNodeBus) -> AVAudioFormat

Retrieves the output format for the bus you specify.

func name(forOutputBus: AVAudioNodeBus) -> String?

Retrieves the name of the output bus you specify.

var numberOfOutputs: Int

The number of output busses for the node.

### Installing and Removing an Audio Tap

func installTap(onBus: AVAudioNodeBus, bufferSize: AVAudioFrameCount, format: AVAudioFormat?, block: AVAudioNodeTapBlock)

Installs an audio tap on a bus you specify to record, monitor, and observe the output of the node.

func removeTap(onBus: AVAudioNodeBus)

Removes an audio tap on a bus you specify.

typealias AVAudioNodeTapBlock

The block that receives copies of the output of an audio node.

### Getting the Audio Engine for the Node

var engine: AVAudioEngine?

The audio engine that manages the node, if any.

### Getting the Latest Node Render Time

var lastRenderTime: AVAudioTime?

The most recent render time.

### Getting Audio Node Properties

var auAudioUnit: AUAudioUnit

An audio unit object that wraps or underlies the implementation’s audio unit.

var latency: TimeInterval

The processing latency of the node, in seconds.

var outputPresentationLatency: TimeInterval

The maximum render pipeline latency downstream of the node, in seconds.

### Resetting the Audio Node

func reset()

Clears a unit’s previous processing state.

### Constants

typealias AVAudioNodeCompletionHandler

A general callback handler for an audio node.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVAudioEnvironmentNode
- AVAudioIONode
- AVAudioMixerNode
- AVAudioPlayerNode
- AVAudioSinkNode
- AVAudioSourceNode
- AVAudioUnit

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Nodes

class AVAudioInputNode

An object that connects to the system’s audio input.

class AVAudioOutputNode

An object that connects to the system’s audio output.

class AVAudioIONode

An object that performs audio input or output in the engine.

