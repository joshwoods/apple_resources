

- Speech
- SFSpeechRecognitionTaskDelegate
-  speechRecognitionTaskFinishedReadingAudio(\_:) 

Instance Method

# speechRecognitionTaskFinishedReadingAudio(\_:)

Tells the delegate when the task is no longer accepting new audio input, even if final processing is in progress.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func speechRecognitionTaskFinishedReadingAudio(_ task: SFSpeechRecognitionTask)
```

## Parameters 

`task`  

The speech recognition task (an SFSpeechRecognitionTask object) that represents the request.

## See Also

### Tracking the Task Progress

func speechRecognitionDidDetectSpeech(SFSpeechRecognitionTask)

Tells the delegate when the task first detects speech in the source audio.

