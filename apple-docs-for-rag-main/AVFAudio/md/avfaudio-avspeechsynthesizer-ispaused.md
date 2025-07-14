

- AVFAudio
- AVSpeechSynthesizer
-  isPaused 

Instance Property

# isPaused

A Boolean value that indicates whether a speech synthesizer is in a paused state.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isPaused: Bool { get }
```

## Discussion

If `true`, the speech synthesizer is in a paused state after beginning to speak an utterance; otherwise, `false`.

## See Also

### Inspecting a speech synthesizer

var isSpeaking: Bool

A Boolean value that indicates whether the speech synthesizer is speaking or is in a paused state and has utterances to speak.

