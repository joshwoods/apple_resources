

- Speech
- SFSpeechRecognitionResult
-  bestTranscription 

Instance Property

# bestTranscription

The transcription with the highest confidence level.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
@NSCopying
var bestTranscription: SFTranscription { get }
```

## See Also

### Getting the Transcriptions

var transcriptions: [SFTranscription]

An array of potential transcriptions, sorted in descending order of confidence.

var speechRecognitionMetadata: SFSpeechRecognitionMetadata?

An object that contains the metadata results for a speech recognition request.

