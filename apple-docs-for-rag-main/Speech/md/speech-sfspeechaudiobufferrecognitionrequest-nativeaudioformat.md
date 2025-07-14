

- Speech
- SFSpeechAudioBufferRecognitionRequest
-  nativeAudioFormat 

Instance Property

# nativeAudioFormat

The preferred audio format for optimal speech recognition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var nativeAudioFormat: AVAudioFormat { get }
```

## Discussion

Use the audio format in this property as a hint for optimal recording, but don’t depend on the value remaining unchanged.

