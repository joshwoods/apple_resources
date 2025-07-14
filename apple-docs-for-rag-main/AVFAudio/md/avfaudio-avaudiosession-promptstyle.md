

- AVFAudio
- AVAudioSession
-  promptStyle 

Instance Property

# promptStyle

A hint to audio sessions that use voice prompt mode to alter the type of prompts they issue in response to other system audio, such as Siri and phone calls.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var promptStyle: AVAudioSession.PromptStyle { get }
```

## Discussion

Apps that issue voice prompts should observe changes in the prompt style and modify their prompts in response. This property is key-value observable.

## See Also

### Inspecting the audio prompt style

enum PromptStyle

Constants that indicate the prompt style to use.

