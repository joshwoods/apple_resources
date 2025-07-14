

- Speech
-  SFSpeechRecognitionResult 

Class

# SFSpeechRecognitionResult

An object that contains the partial or final results of a speech recognition request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class SFSpeechRecognitionResult
```

## Overview

Use an `SFSpeechRecognitionResult` object to retrieve the results of a speech recognition request. You don’t create these objects directly. Instead, the Speech framework creates them and passes them to the handler block or delegate object you specified when starting your speech recognition task.

A speech recognition result object contains one or more transcriptions of the current utterance. Each transcription has a confidence rating indicating how likely it is to be correct. You can also get the transcription with the highest rating directly from the bestTranscription property.

If you requested partial results from the speech recognizer, the transcriptions may represent only part of the total audio content. Use the isFinal property to determine if the request contains partial or final results.

## Topics

### Getting the Transcriptions

var bestTranscription: SFTranscription

The transcription with the highest confidence level.

var transcriptions: [SFTranscription]

An array of potential transcriptions, sorted in descending order of confidence.

var speechRecognitionMetadata: SFSpeechRecognitionMetadata?

An object that contains the metadata results for a speech recognition request.

### Determining Whether the Transcriptions Are Final

var isFinal: Bool

A Boolean value that indicates whether speech recognition is complete and whether the transcriptions are final.

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

class SFSpeechRecognitionMetadata

The metadata of speech in the audio of a speech recognition request.

class SFTranscription

A textual representation of the specified speech in its entirety, as recognized by the speech recognizer.

class SFTranscriptionSegment

A discrete part of an entire transcription, as identified by the speech recognizer.

