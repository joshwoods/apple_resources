

- Speech
- SFSpeechRecognitionTask
-  state 

Instance Property

# state

The current state of the speech recognition task.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var state: SFSpeechRecognitionTaskState { get }
```

## Discussion

Check the value of this property to get the state of the in-progress speech recognition session. For valid values, see SFSpeechRecognitionTaskState.

## See Also

### Monitoring Recognition Progress

enum SFSpeechRecognitionTaskState

The state of the task associated with the recognition request.

var error: (any Error)?

An error object that specifies the error that occurred during a speech recognition task.

