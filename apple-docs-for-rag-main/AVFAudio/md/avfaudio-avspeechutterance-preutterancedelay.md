

- AVFAudio
- AVSpeechUtterance
-  preUtteranceDelay 

Instance Property

# preUtteranceDelay

The amount of time the speech synthesizer pauses before speaking the utterance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var preUtteranceDelay: TimeInterval { get set }
```

## Discussion

When multiple utterances exist in the queue, the speech synthesizer pauses a minimum amount of time equal to the sum of the current utterance’s postUtteranceDelay and the next utterance’s `preUtteranceDelay`.

## See Also

### Configuring utterance timing

var rate: Float

The rate the speech synthesizer uses when speaking the utterance.

let AVSpeechUtteranceMinimumSpeechRate: Float

The minimum rate the speech synthesizer uses when speaking an utterance.

let AVSpeechUtteranceMaximumSpeechRate: Float

The maximum rate the speech synthesizer uses when speaking an utterance.

let AVSpeechUtteranceDefaultSpeechRate: Float

The default rate the speech synthesizer uses when speaking an utterance.

var postUtteranceDelay: TimeInterval

The amount of time the speech synthesizer pauses after speaking an utterance before handling the next utterance in the queue.

