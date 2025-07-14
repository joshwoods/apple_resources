

- Speech
- SFSpeechRecognitionTaskDelegate
-  speechRecognitionDidDetectSpeech(\_:) 

Instance Method

# speechRecognitionDidDetectSpeech(\_:)

Tells the delegate when the task first detects speech in the source audio.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func speechRecognitionDidDetectSpeech(_ task: SFSpeechRecognitionTask)
```

## Parameters 

`task`  

The speech recognition task (an SFSpeechRecognitionTask object) that represents the request.

## See Also

### Tracking the Task Progress

func speechRecognitionTaskFinishedReadingAudio(SFSpeechRecognitionTask)

Tells the delegate when the task is no longer accepting new audio input, even if final processing is in progress.

