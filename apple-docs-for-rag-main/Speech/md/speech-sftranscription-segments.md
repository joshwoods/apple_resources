

- Speech
- SFTranscription
-  segments 

Instance Property

# segments

An array of transcription segments that represent the parts of the transcription, as identified by the speech recognizer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var segments: [SFTranscriptionSegment] { get }
```

## Discussion

The order of the segments in the array matches the order in which the corresponding utterances occur in the spoken content.

