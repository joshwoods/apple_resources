

- Speech
- SFSpeechRecognitionTask
-  isFinishing 

Instance Property

# isFinishing

A Boolean value that indicates whether audio input has stopped.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var isFinishing: Bool { get }
```

## Discussion

By default, the value of this property is `false`.

## See Also

### Finishing a Speech Recognition Task

func finish()

Stops accepting new audio and finishes processing on the audio input that has already been accepted.

