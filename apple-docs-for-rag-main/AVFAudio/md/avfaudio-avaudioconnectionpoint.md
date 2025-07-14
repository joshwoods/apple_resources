

- AVFAudio
-  AVAudioConnectionPoint 

Class

# AVAudioConnectionPoint

A representation of either a source or destination connection point in the audio engine.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioConnectionPoint
```

## Overview

Instances of this class are immutable.

## Topics

### Creating a Connection Point

init(node: AVAudioNode, bus: AVAudioNodeBus)

Creates a connection point object.

### Getting Connection Point Properties

func inputConnectionPoint(for: AVAudioNode, inputBus: AVAudioNodeBus) -> AVAudioConnectionPoint?

Returns connection information about a node’s input bus.

func outputConnectionPoints(for: AVAudioNode, outputBus: AVAudioNodeBus) -> [AVAudioConnectionPoint]

Returns connection information about a node’s output bus.

var bus: AVAudioNodeBus

The bus on the node in the connection point.

var node: AVAudioNode?

The node in the connection point.

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

### Using Connection Points

func connect(AVAudioNode, to: [AVAudioConnectionPoint], fromBus: AVAudioNodeBus, format: AVAudioFormat?)

Establishes a connection between a source node and multiple destination nodes.

