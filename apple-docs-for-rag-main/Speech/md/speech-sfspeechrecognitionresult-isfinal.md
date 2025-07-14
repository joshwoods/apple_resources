

- Speech
- SFSpeechRecognitionResult
-  isFinal 

Instance Property

# isFinal

A Boolean value that indicates whether speech recognition is complete and whether the transcriptions are final.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var isFinal: Bool { get }
```

## Discussion

When a speech recognition request is final, its transcriptions don’t change.

