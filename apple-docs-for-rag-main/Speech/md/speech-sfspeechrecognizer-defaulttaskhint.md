

- Speech
- SFSpeechRecognizer
-  defaultTaskHint 

Instance Property

# defaultTaskHint

A hint that indicates the type of speech recognition being requested.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var defaultTaskHint: SFSpeechRecognitionTaskHint { get set }
```

## Discussion

By default, the value of this property overrides the SFSpeechRecognitionTaskHint.unspecified value for requests. For possible values, see SFSpeechRecognitionTaskHint.

## See Also

### Configuring the Speech Recognizer

var queue: OperationQueue

The queue on which to execute recognition task handlers and delegate methods.

