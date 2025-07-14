

- AVFAudio
- AVSpeechSynthesizerDelegate
-  speechSynthesizer(\_:didFinish:) 

Instance Method

# speechSynthesizer(\_:didFinish:)

Tells the delegate when the synthesizer finishes speaking an utterance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
optional func speechSynthesizer(
    _ synthesizer: AVSpeechSynthesizer,
    didFinish utterance: AVSpeechUtterance
)
```

## Parameters 

`synthesizer`  

The speech synthesizer that finishes speaking the utterance.

`utterance`  

The utterance that the speech synthesizer finishes speaking.

## Discussion

The system ignores the final utterance’s postUtteranceDelay and calls this method immediately when speech ends.

## See Also

### Responding to speech synthesis events

func speechSynthesizer(AVSpeechSynthesizer, didStart: AVSpeechUtterance)

Tells the delegate when the synthesizer begins speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, willSpeakRangeOfSpeechString: NSRange, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a portion of an utterance’s text.

func speechSynthesizer(AVSpeechSynthesizer, willSpeak: AVSpeechSynthesisMarker, utterance: AVSpeechUtterance)

Tells the delegate when the synthesizer is about to speak a marker of an utterance’s text.

func speechSynthesizer(AVSpeechSynthesizer, didPause: AVSpeechUtterance)

Tells the delegate when the synthesizer pauses while speaking an utterance.

func speechSynthesizer(AVSpeechSynthesizer, didContinue: AVSpeechUtterance)

Tells the delegate when the synthesizer resumes speaking an utterance after pausing.

func speechSynthesizer(AVSpeechSynthesizer, didCancel: AVSpeechUtterance)

Tells the delegate when the synthesizer cancels speaking an utterance.

