

- AVFAudio
-  AVAudioMixing 

Protocol

# AVAudioMixing

A collection of properties that are applicable to the input bus of a mixer node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol AVAudioMixing : AVAudio3DMixing, AVAudioStereoMixing
```

## Overview

Nodes that conform to the `AVAudioMixing` protocol can talk to a mixer node downstream. This is specific to the classes AVAudioMixerNode and AVAudioEnvironmentNode. Effect nodes can’t talk to their downstream mixer.

When connecting a source node, the properties that this protocol defines apply to the respective input bus of the mixer.

You can change the state of properties before connecting a source node to the mixer. The system caches your changes and applies them upon connection. It caches the properties again after disconnection.

Source nodes maintain mixing settings when switching between different mixers. For example, an AVAudioPlayerNode, in a gaming scenario, can set up 3D mixing settings and then move from one environment to another.

Important

Several classes adopt the `AVAudioMixing` protocol. The protocol itself conforms to AVAudio3DMixing and AVAudioStereoMixing. Classes that conform to `AVAudioMixing` also conform to those protocols.

## Topics

### Defining Mixing Properties

protocol AVAudioStereoMixing

A protocol that defines stereo mixing properties a mixer uses.

protocol AVAudio3DMixing

A collection of properties that define 3D mixing properties.

### Getting and Setting the Destination

class AVAudioMixingDestination

An object that represents a connection to a mixer node from a node that conforms to the audio mixing protocol.

func destination(forMixer: AVAudioNode, bus: AVAudioNodeBus) -> AVAudioMixingDestination?

Gets the audio mixing destination object that corresponds to the specified mixer node and input bus.

**Required**

### Getting and Setting the Bus Volume

var volume: Float

The bus’s input volume.

**Required**

## Relationships

### Inherits From

- AVAudio3DMixing
- AVAudioStereoMixing
- NSObjectProtocol

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

### Mixing

class AVAudioMixerNode

An object that takes any number of inputs and converts them into a single output.

