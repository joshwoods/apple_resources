

- Speech
-  SFTranscription 

Class

# SFTranscription

A textual representation of the specified speech in its entirety, as recognized by the speech recognizer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class SFTranscription
```

## Overview

Use `SFTranscription` to obtain all the recognized utterances from your audio content. An *utterance* is a vocalized word or group of words that represent a single meaning to the speech recognizer (SFSpeechRecognizer).

Use the formattedString property to retrieve the entire transcription of utterances, or use the segments property to retrieve an individual utterance (SFTranscriptionSegment).

You don’t create an `SFTranscription` directly. Instead, you retrieve it from an SFSpeechRecognitionResult instance. The speech recognizer sends a speech recognition result to your app in one of two ways, depending on how your app started a speech recognition task.

You can start a speech recognition task by using the speech recognizer’s recognitionTask(with:resultHandler:) method. When the task is complete, the speech recognizer sends an SFSpeechRecognitionResult instance to your `resultHandler` closure. Alternatively, you can use the speech recognizer’s recognitionTask(with:delegate:) method to start a speech recognition task. When the task is complete, the speech recognizer uses your SFSpeechRecognitionTaskDelegate to send an SFSpeechRecognitionResult by using the delegate’s speechRecognitionTask(_:didFinishRecognition:) method.

An `SFTranscription` represents only a potential version of the speech. It might not be an accurate representation of the utterances.

## Topics

### Transcribing the Utterances

var formattedString: String

The entire transcription of utterances, formatted into a single, user-displayable string.

### Getting Individual Utterances

var segments: [SFTranscriptionSegment]

An array of transcription segments that represent the parts of the transcription, as identified by the speech recognizer.

### Deprecated

var averagePauseDuration: TimeInterval

The average pause duration between words, measured in seconds.

Deprecated

var speakingRate: Double

The number of words spoken per minute.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Transcription results

class SFSpeechRecognitionResult

An object that contains the partial or final results of a speech recognition request.

class SFSpeechRecognitionMetadata

The metadata of speech in the audio of a speech recognition request.

class SFTranscriptionSegment

A discrete part of an entire transcription, as identified by the speech recognizer.

