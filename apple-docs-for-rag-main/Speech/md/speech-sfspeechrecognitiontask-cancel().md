

- Speech
- SFSpeechRecognitionTask
-  cancel() 

Instance Method

# cancel()

Cancels the current speech recognition task.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func cancel()
```

## Discussion

You can cancel recognition tasks for both prerecorded and live audio input. For example, you might cancel a task in response to a user action or because the recording was interrupted.

When canceling a task, be sure to release any resources associated with the task, such as the audio input resources you are using to capture audio samples.

## See Also

### Canceling a Speech Recognition Task

var isCancelled: Bool

A Boolean value that indicates whether the speech recognition task was canceled.

