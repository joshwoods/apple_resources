

- Speech
- SFSpeechRecognitionTaskDelegate
-  speechRecognitionTask(\_:didHypothesizeTranscription:) 

Instance Method

# speechRecognitionTask(\_:didHypothesizeTranscription:)

Tells the delegate that a hypothesized transcription is available.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func speechRecognitionTask(
    _ task: SFSpeechRecognitionTask,
    didHypothesizeTranscription transcription: SFTranscription
)
```

## Parameters 

`task`  

The speech recognition task (an SFSpeechRecognitionTask object) that represents the request.

`transcription`  

The hypothesized transcription in an SFTranscription object.

## Discussion

This method is called for all recognitions, including partial recognitions.

