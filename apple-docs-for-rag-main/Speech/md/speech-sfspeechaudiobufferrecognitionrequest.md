

- Speech
-  SFSpeechAudioBufferRecognitionRequest 

Class

# SFSpeechAudioBufferRecognitionRequest

A request to recognize speech from captured audio content, such as audio from the device’s microphone.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class SFSpeechAudioBufferRecognitionRequest
```

## Overview

Use an SFSpeechAudioBufferRecognitionRequest object to perform speech recognition on live audio, or on a set of existing audio buffers. For example, use this request object to route audio from a device’s microphone to the speech recognizer.

The request object contains no audio initially. As you capture audio, call append(_:) or appendAudioSampleBuffer(_:) to add audio samples to the request object. The speech recognizer continuously analyzes the audio you appended, stopping only when you call the endAudio() method. You must call endAudio() explicitly to stop the speech recognition process.

For a complete example of how to use audio buffers with speech recognition, see SpeakToMe: Using Speech Recognition with AVAudioEngine.

## Topics

### Appending Audio Buffers

func append(AVAudioPCMBuffer)

Appends audio in the PCM format to the end of the recognition request.

func appendAudioSampleBuffer(CMSampleBuffer)

Appends audio to the end of the recognition request.

func endAudio()

Marks the end of audio input for the recognition request.

### Getting the Audio Format

var nativeAudioFormat: AVAudioFormat

The preferred audio format for optimal speech recognition.

## Relationships

### Inherits From

- SFSpeechRecognitionRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio sources

Recognizing speech in live audio

Perform speech recognition on audio coming from the microphone of an iOS device.

class SFSpeechURLRecognitionRequest

A request to recognize speech in a recorded audio file.

class SFSpeechRecognitionRequest

An abstract class that represents a request to recognize speech from an audio source.

