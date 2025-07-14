

- Speech
-  SFSpeechRecognitionMetadata 

Class

# SFSpeechRecognitionMetadata

The metadata of speech in the audio of a speech recognition request.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
class SFSpeechRecognitionMetadata
```

## Topics

### Getting the Audio Timing Information

var averagePauseDuration: TimeInterval

The average pause duration between words, measured in seconds.

var speakingRate: Double

The number of words spoken per minute.

var speechDuration: TimeInterval

The duration in seconds of speech in the audio.

var speechStartTimestamp: TimeInterval

The start timestamp of speech in the audio.

### Analyzing Voice

var voiceAnalytics: SFVoiceAnalytics?

An analysis of the transcription segment’s vocal properties.

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

class SFTranscription

A textual representation of the specified speech in its entirety, as recognized by the speech recognizer.

class SFTranscriptionSegment

A discrete part of an entire transcription, as identified by the speech recognizer.

