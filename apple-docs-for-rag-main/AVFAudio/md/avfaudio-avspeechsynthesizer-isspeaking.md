

- AVFAudio
- AVSpeechSynthesizer
-  isSpeaking 

Instance Property

# isSpeaking

A Boolean value that indicates whether the speech synthesizer is speaking or is in a paused state and has utterances to speak.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isSpeaking: Bool { get }
```

## Discussion

If `true`, the synthesizer is speaking or is in a paused state with utterances in its queue. If `false`, the synthesizer isn’t speaking and it doesn’t have any utterances in its queue.

## See Also

### Inspecting a speech synthesizer

var isPaused: Bool

A Boolean value that indicates whether a speech synthesizer is in a paused state.

