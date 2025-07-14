

- Speech
- SFSpeechRecognitionResult
-  speechRecognitionMetadata 

Instance Property

# speechRecognitionMetadata

An object that contains the metadata results for a speech recognition request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var speechRecognitionMetadata: SFSpeechRecognitionMetadata? { get }
```

## See Also

### Getting the Transcriptions

var bestTranscription: SFTranscription

The transcription with the highest confidence level.

var transcriptions: [SFTranscription]

An array of potential transcriptions, sorted in descending order of confidence.

