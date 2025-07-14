

- AVFAudio
-  AVSpeechSynthesisProviderAudioUnit 

Class

# AVSpeechSynthesisProviderAudioUnit

An object that generates speech from text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVSpeechSynthesisProviderAudioUnit
```

## Overview

Use a speech synthesizer audio unit to generate audio buffers that contain speech for a given voice and speech markup. The audio unit receives an AVSpeechSynthesisProviderRequest as input, and extracts audio buffers through the render block.

Use speechSynthesisOutputMetadataBlock to provide metadata as an array of AVSpeechSynthesisMarker.

The system scans and loads voices for audio unit extensions of this type, and the voices it provides are available for use in AVSpeechSynthesizer and accessibility technologies like VoiceOver and Speak Screen.

Important

Network access isn’t allowed in speech synthesizers.

## Topics

### Rendering speech

func synthesizeSpeechRequest(AVSpeechSynthesisProviderRequest)

Sets the text to synthesize and the voice to use.

class AVSpeechSynthesisProviderRequest

An object that represents the text to synthesize and the voice to use.

### Supplying metadata

typealias AVSpeechSynthesisProviderOutputBlock

A type that represents the method for sending marker information to the host.

var speechSynthesisOutputMetadataBlock: AVSpeechSynthesisProviderOutputBlock?

A block that subclasses use to send marker information to the host.

class AVSpeechSynthesisMarker

An object that contains information about the synthesized audio.

### Getting and setting voices

var speechVoices: [AVSpeechSynthesisProviderVoice]

A list of voices the audio unit provides to the system.

class AVSpeechSynthesisProviderVoice

An object that represents a voice that an audio unit provides to its host.

### Cancelling a request

func cancelSpeechRequest()

Informs the audio unit to discard the speech request.

## Relationships

### Inherits From

- AUAudioUnit

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

