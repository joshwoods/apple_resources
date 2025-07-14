

- AVFAudio
-  AVSpeechUtteranceDefaultSpeechRate 

Global Variable

# AVSpeechUtteranceDefaultSpeechRate

The default rate the speech synthesizer uses when speaking an utterance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
let AVSpeechUtteranceDefaultSpeechRate: Float
```

## Discussion

The speech rate is a decimal representation.

## See Also

### Configuring utterance timing

var rate: Float

The rate the speech synthesizer uses when speaking the utterance.

let AVSpeechUtteranceMinimumSpeechRate: Float

The minimum rate the speech synthesizer uses when speaking an utterance.

let AVSpeechUtteranceMaximumSpeechRate: Float

The maximum rate the speech synthesizer uses when speaking an utterance.

var preUtteranceDelay: TimeInterval

The amount of time the speech synthesizer pauses before speaking the utterance.

var postUtteranceDelay: TimeInterval

The amount of time the speech synthesizer pauses after speaking an utterance before handling the next utterance in the queue.

