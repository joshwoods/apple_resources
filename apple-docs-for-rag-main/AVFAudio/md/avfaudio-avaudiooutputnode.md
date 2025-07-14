

- AVFAudio
-  AVAudioOutputNode 

Class

# AVAudioOutputNode

An object that connects to the system’s audio output.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioOutputNode
```

## Overview

This node connects to the system’s audio output when rendering to or from an audio device. This node performs output in response to client’s requests when the engine is in manual rendering mode.

This audio node has one element. The format of the output scope reflects:

- The audio hardware sample rate and channel count when it connects to the hardware.

- The engine’s manual rendering mode output format (see manualRenderingFormat).

The format of the input scope is initially the same as that of the output, but you may set it to a different format, in which case the audio node converts.

Important

This class has no methods of its own. It overrides methods that its base classes define.

## Relationships

### Inherits From

- AVAudioIONode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Nodes

class AVAudioNode

An object you use for audio generation, processing, or an I/O block.

class AVAudioInputNode

An object that connects to the system’s audio input.

class AVAudioIONode

An object that performs audio input or output in the engine.

