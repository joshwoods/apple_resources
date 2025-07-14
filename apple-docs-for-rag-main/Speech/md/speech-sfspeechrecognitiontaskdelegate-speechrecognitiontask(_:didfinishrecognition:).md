

- Speech
- SFSpeechRecognitionTaskDelegate
-  speechRecognitionTask(\_:didFinishRecognition:) 

Instance Method

# speechRecognitionTask(\_:didFinishRecognition:)

Tells the delegate when the final utterance is recognized.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func speechRecognitionTask(
    _ task: SFSpeechRecognitionTask,
    didFinishRecognition recognitionResult: SFSpeechRecognitionResult
)
```

## Parameters 

`task`  

The speech recognition task (an SFSpeechRecognitionTask object) that represents the request.

`recognitionResult`  

A recognized utterance that contains one or more transcription hypotheses in an SFSpeechRecognitionResult object.

## Discussion

When this method is called, the delegate should expect no further information about the utterance to be reported.

## See Also

### Finishing a Speech Recognition Task

func speechRecognitionTask(SFSpeechRecognitionTask, didFinishSuccessfully: Bool)

Tells the delegate when the recognition of all requested utterances is finished.

func speechRecognitionTaskWasCancelled(SFSpeechRecognitionTask)

Tells the delegate that the task has been canceled.

