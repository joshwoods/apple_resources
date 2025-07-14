

- AVFAudio
- AVSpeechUtterance
-  rate 

Instance Property

# rate

The rate the speech synthesizer uses when speaking the utterance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var rate: Float { get set }
```

## Discussion

The speech rate is a decimal representation within the range of AVSpeechUtteranceMinimumSpeechRate and AVSpeechUtteranceMaximumSpeechRate. Lower values correspond to slower speech, and higher values correspond to faster speech. The default value is AVSpeechUtteranceDefaultSpeechRate. Set this property before enqueing the utterance because setting it afterward has no effect.

## See Also

### Configuring utterance timing

let AVSpeechUtteranceMinimumSpeechRate: Float

The minimum rate the speech synthesizer uses when speaking an utterance.

let AVSpeechUtteranceMaximumSpeechRate: Float

The maximum rate the speech synthesizer uses when speaking an utterance.

let AVSpeechUtteranceDefaultSpeechRate: Float

The default rate the speech synthesizer uses when speaking an utterance.

var preUtteranceDelay: TimeInterval

The amount of time the speech synthesizer pauses before speaking the utterance.

var postUtteranceDelay: TimeInterval

The amount of time the speech synthesizer pauses after speaking an utterance before handling the next utterance in the queue.

