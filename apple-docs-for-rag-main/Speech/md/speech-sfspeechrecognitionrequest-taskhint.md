

- Speech
- SFSpeechRecognitionRequest
-  taskHint 

Instance Property

# taskHint

A value that indicates the type of speech recognition being performed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var taskHint: SFSpeechRecognitionTaskHint { get set }
```

## Discussion

The default value of this property is SFSpeechRecognitionTaskHint.unspecified. For a valid list of values, see SFSpeechRecognitionTaskHint.

## See Also

### Speech Type Classification

enum SFSpeechRecognitionTaskHint

The type of task for which you are using speech recognition.

