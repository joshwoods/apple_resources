

- AVFAudio
-  AVAudioMixingDestination 

Class

# AVAudioMixingDestination

An object that represents a connection to a mixer node from a node that conforms to the audio mixing protocol.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioMixingDestination
```

## Overview

You can only use a destination instance when a source node provides it. You can’t use it as a standalone instance.

## Topics

### Getting Mixing Destination Properties

var connectionPoint: AVAudioConnectionPoint

The underlying mixer connection point.

## Relationships

### Inherits From

- NSObject

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

### Getting and Setting the Destination

func destination(forMixer: AVAudioNode, bus: AVAudioNodeBus) -> AVAudioMixingDestination?

Gets the audio mixing destination object that corresponds to the specified mixer node and input bus.

**Required**

