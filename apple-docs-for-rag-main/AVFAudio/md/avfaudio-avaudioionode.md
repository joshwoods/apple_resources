

- AVFAudio
-  AVAudioIONode 

Class

# AVAudioIONode

An object that performs audio input or output in the engine.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioIONode
```

## Overview

When rendering to and from an audio device in macOS, AVAudioInputNode and AVAudioOutputNode communicate with the system’s default input and output devices. In iOS, they communicate with the devices appropriate to the app’s AVAudioSession category, configurations, and user actions, such as connecting or disconnecting external devices.

In the manual rendering mode, AVAudioInputNode and AVAudioOutputNode perform the input and output in the engine in response to the client’s request.

## Topics

### Getting the Audio Unit

var audioUnit: AudioUnit?

The node’s underlying audio unit, if any.

### Getting the I/O Latency

var presentationLatency: TimeInterval

The presentation or hardware latency, applicable when rendering to or from an audio device.

### Getting and Setting the Voice Processing State

func setVoiceProcessingEnabled(Bool) throws

Enables or disables voice processing on the I/O node.

var isVoiceProcessingEnabled: Bool

A Boolean value that indicates whether voice processing is in an enabled state.

## Relationships

### Inherits From

- AVAudioNode

### Inherited By

- AVAudioInputNode
- AVAudioOutputNode

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

class AVAudioOutputNode

An object that connects to the system’s audio output.

