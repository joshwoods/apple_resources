

- Speech
-  SFSpeechRecognitionRequest 

Class

# SFSpeechRecognitionRequest

An abstract class that represents a request to recognize speech from an audio source.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class SFSpeechRecognitionRequest
```

## Overview

Don’t create SFSpeechRecognitionRequest objects directly. Create an SFSpeechURLRecognitionRequest or SFSpeechAudioBufferRecognitionRequest object instead. Use the properties of this class to configure various aspects of your request object before you start the speech recognition process. For example, use the shouldReportPartialResults property to specify whether you want partial results or only the final result of speech recognition.

## Topics

### Recognition Request Configuration

var requiresOnDeviceRecognition: Bool

A Boolean value that determines whether a request must keep its audio data on the device.

var shouldReportPartialResults: Bool

A Boolean value that indicates whether you want intermediate results returned for each utterance.

var contextualStrings: [String]

An array of phrases that should be recognized, even if they are not in the system vocabulary.

### Speech Type Classification

var taskHint: SFSpeechRecognitionTaskHint

A value that indicates the type of speech recognition being performed.

enum SFSpeechRecognitionTaskHint

The type of task for which you are using speech recognition.

### Punctuation

var addsPunctuation: Bool

A Boolean value that indicates whether to add punctuation to speech recognition results.

### Deprecated

var interactionIdentifier: String?

An identifier string that you use to describe the type of interaction associated with the speech recognition request.

Deprecated

### Instance Properties

var customizedLanguageModel: SFSpeechLanguageModel.Configuration?

## Relationships

### Inherits From

- NSObject

### Inherited By

- SFSpeechAudioBufferRecognitionRequest
- SFSpeechURLRecognitionRequest

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

class SFSpeechAudioBufferRecognitionRequest

A request to recognize speech from captured audio content, such as audio from the device’s microphone.

