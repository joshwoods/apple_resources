

- AVFAudio
-  AVAudioInputNode 

Class

# AVAudioInputNode

An object that connects to the system’s audio input.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class AVAudioInputNode
```

## Overview

This node connects to the system’s audio input when rendering to or from an audio device. In manual rendering mode, this node supplies input data to the engine.

This audio node has one element. The format of the input scope reflects:

- The audio hardware sample rate and channel count when it connects to hardware.

- The format of the PCM audio data that the node supplies to the engine in manual rendering mode. For more information, see setManualRenderingInputPCMFormat(_:inputBlock:)

When rendering from an audio device, the input node doesn’t support format conversion. In this case, the format of the output scope must be the same as the input and the formats for all nodes connected to the input chain.

In manual rendering mode, the format of the output scope is initially the same as the input, but you may set it to a different format, which converts the node.

Important

This class has no methods of its own. It implements the methods that the AVAudioMixing protocol defines, as well as those of the AVAudio3DMixing protocol, which the AVAudioMixing protocol adopts. For more information, see AVAudioMixing and AVAudio3DMixing.

## Topics

### Manually Giving Data to an Audio Engine

func setManualRenderingInputPCMFormat(AVAudioFormat, inputBlock: AVAudioIONodeInputBlock) -> Bool

Supplies the data through the input node to the engine while operating in the manual rendering mode.

typealias AVAudioIONodeInputBlock

The type that represents a block to render operation calls to get input data when in manual rendering mode.

### Getting and Setting Voice Processing Properties

var isVoiceProcessingInputMuted: Bool

A Boolean that indicates whether the input of the voice processing unit is in a muted state.

var isVoiceProcessingBypassed: Bool

A Boolean that indicates whether the node bypasses all microphone uplink processing of the voice-processing unit.

var isVoiceProcessingAGCEnabled: Bool

A Boolean that indicates whether automatic gain control on the processed microphone uplink signal is active.

var voiceProcessingOtherAudioDuckingConfiguration: AVAudioVoiceProcessingOtherAudioDuckingConfiguration

The ducking configuration of nonvoice audio.

struct AVAudioVoiceProcessingOtherAudioDuckingConfiguration

The configuration of ducking non-voice audio.

### Handling Muted Speech Events

func setMutedSpeechActivityEventListener(((AVAudioVoiceProcessingSpeechActivityEvent) -> Void)?) -> Bool

enum AVAudioVoiceProcessingSpeechActivityEvent

Types of speech activity events.

## Relationships

### Inherits From

- AVAudioIONode

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

### Nodes

class AVAudioNode

An object you use for audio generation, processing, or an I/O block.

class AVAudioOutputNode

An object that connects to the system’s audio output.

class AVAudioIONode

An object that performs audio input or output in the engine.

