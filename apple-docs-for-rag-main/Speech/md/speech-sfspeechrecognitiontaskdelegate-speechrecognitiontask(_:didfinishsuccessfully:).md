

- Speech
- SFSpeechRecognitionTaskDelegate
-  speechRecognitionTask(\_:didFinishSuccessfully:) 

Instance Method

# speechRecognitionTask(\_:didFinishSuccessfully:)

Tells the delegate when the recognition of all requested utterances is finished.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func speechRecognitionTask(
    _ task: SFSpeechRecognitionTask,
    didFinishSuccessfully successfully: Bool
)
```

## Parameters 

`task`  

The speech recognition task (an SFSpeechRecognitionTask object) that represents the request.

`successfully`  

A Boolean value that indicates whether the task was successful. When this parameter is false, use the error property of the task to get information about why the task was unsuccessful.

## See Also

### Finishing a Speech Recognition Task

func speechRecognitionTask(SFSpeechRecognitionTask, didFinishRecognition: SFSpeechRecognitionResult)

Tells the delegate when the final utterance is recognized.

func speechRecognitionTaskWasCancelled(SFSpeechRecognitionTask)

Tells the delegate that the task has been canceled.

