

- Speech
- SFSpeechRecognitionResult
-  transcriptions 

Instance Property

# transcriptions

An array of potential transcriptions, sorted in descending order of confidence.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var transcriptions: [SFTranscription] { get }
```

## Discussion

All transcriptions correspond to the same utterance, which can be a partial or final result of the overall request. The first transcription in the array has the highest confidence rating, followed by transcriptions with decreasing confidence ratings.

## See Also

### Getting the Transcriptions

var bestTranscription: SFTranscription

The transcription with the highest confidence level.

var speechRecognitionMetadata: SFSpeechRecognitionMetadata?

An object that contains the metadata results for a speech recognition request.

