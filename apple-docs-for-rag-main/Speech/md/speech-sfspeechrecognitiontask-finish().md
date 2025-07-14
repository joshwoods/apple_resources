

- Speech
- SFSpeechRecognitionTask
-  finish() 

Instance Method

# finish()

Stops accepting new audio and finishes processing on the audio input that has already been accepted.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func finish()
```

## Discussion

For audio buffer–based recognition, recognition does not finish until this method is called, so be sure to call it when the audio source is exhausted.

## See Also

### Finishing a Speech Recognition Task

var isFinishing: Bool

A Boolean value that indicates whether audio input has stopped.

