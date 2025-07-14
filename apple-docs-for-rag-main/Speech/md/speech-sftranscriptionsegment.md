

- Speech
-  SFTranscriptionSegment 

Class

# SFTranscriptionSegment

A discrete part of an entire transcription, as identified by the speech recognizer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class SFTranscriptionSegment
```

## Overview

Use SFTranscriptionSegment to get details about a part of an overall SFTranscription. An SFTranscriptionSegment represents an utterance, which is a vocalized word or group of words that represent a single meaning to the speech recognizer (SFSpeechRecognizer).

You don’t create transcription object segments directly. Instead, you access them from a transcription’s segments property.

A transcription segment includes the following information:

- The text of the utterance, plus any alternative interpretations of the spoken word.

- The character range of the segment within the formattedString of its parent SFTranscription.

- A confidence value, indicating how likely it is that the specified string matches the audible speech.

- A timestamp and duration value, indicating the position of the segment within the provided audio stream.

## Topics

### Transcribing the Segment

var substring: String

The string representation of the utterance in the transcription segment.

var substringRange: NSRange

The range information for the transcription segment’s substring, relative to the overall transcription.

var alternativeSubstrings: [String]

An array of alternate interpretations of the utterance in the transcription segment.

### Assessing the Recognition Confidence Level

var confidence: Float

The level of confidence the speech recognizer has in its recognition of the speech transcribed for the segment.

### Getting the Audio Timing Information

var timestamp: TimeInterval

The start time of the segment in the processed audio stream.

var duration: TimeInterval

The number of seconds it took for the user to speak the utterance represented by the segment.

### Deprecated

var voiceAnalytics: SFVoiceAnalytics?

An analysis of the transcription segment’s vocal properties.

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

class SFTranscription

A textual representation of the specified speech in its entirety, as recognized by the speech recognizer.

