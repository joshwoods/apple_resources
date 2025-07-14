

- Speech
- SFSpeechRecognitionTaskDelegate
-  speechRecognitionTaskWasCancelled(\_:) 

Instance Method

# speechRecognitionTaskWasCancelled(\_:)

Tells the delegate that the task has been canceled.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func speechRecognitionTaskWasCancelled(_ task: SFSpeechRecognitionTask)
```

## Parameters 

`task`  

The speech recognition task (an SFSpeechRecognitionTask object) that represents the request.

## Discussion

A speech recognition task can be canceled by the user, by your app, or by the system.

## See Also

### Finishing a Speech Recognition Task

func speechRecognitionTask(SFSpeechRecognitionTask, didFinishRecognition: SFSpeechRecognitionResult)

Tells the delegate when the final utterance is recognized.

func speechRecognitionTask(SFSpeechRecognitionTask, didFinishSuccessfully: Bool)

Tells the delegate when the recognition of all requested utterances is finished.

